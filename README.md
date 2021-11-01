# DigitalElectronics2_Lab6
LCD

## Link to GitHub and name:

Link to GitHub: https://github.com/raulgoi/DigitalElectronics_Lab6
Raúl Gómez Ibáñez.

## LCD display module

### Code ASCII

* ASCII: American Standard Code for Information Interchange, is a relationship between a normal character and its code for electronic comunication. It is a code that uses numbers to represent characters. Each letter is assigned a number between 0 and 127. A upper and lower case character are assigned different numbers. It can be used in computers, telecomunications equipment and services relationated with technology. The most of the codes that are used in this days, are based in the ASCII. There is a table where you can see the relation.

### Signals of De2

D = 01000100
e = 0 1100101
2 = 00110010

![De2](https://user-images.githubusercontent.com/91128806/139685422-df2a828e-553d-418a-9538-f1fdd9966ed2.jpeg)




## Stopwatch


![Flowchart](https://user-images.githubusercontent.com/91128806/139685056-55de3e87-b963-4877-bb05-35230b3e0618.png)




## Custom characters


     /* Variables ---------------------------------------------------------*/
     // Custom character definition
     uint8_t customChar[16] = {
     
     	
	  0b11110,
    	  0b10010,
       	  0b10010,
    	  0b11110,
    	  0b11000,
   	  0b10100,
   	  0b10010,
   	  0b00000,
          0b11111,
	  0b10001,
  	  0b10001,
  	  0b11111,
  	  0b10001,
  	  0b10001,
  	  0b10001,
  	  0b00000
      
       };
       int main(void)
    {
    
    lcd_init(LCD_DISP_ON);
    lcd_command(1 << LCD_CGRAM);
    for (uint8_t i = 0; i < 16; i++)
    {
      lcd_data(customChar[i]);
     }
   
     lcd_command(1 << LCD_DDRAM);
     lcd_putc(0);
       
       
 
 ## Picture of the kitchen clock
 
 
 ![Captura de pantalla LAB 6](https://user-images.githubusercontent.com/91128806/139667509-18f62d60-339d-4b62-b308-1d13c1dcca80.png)

