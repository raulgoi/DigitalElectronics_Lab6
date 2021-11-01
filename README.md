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

![De2](https://user-images.githubusercontent.com/91128806/139091917-69324857-7e27-4a09-b17a-ca0dd2479c96.jpeg)


## Stopwatch


![Flowchart](https://user-images.githubusercontent.com/91128806/139658816-953b46aa-537e-4a38-967c-d911f12e27cd.png)



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
