# A Digital Timer!



## Part A. Solder your LCD panel

![The soldered panel](solderedPanel.JPG)

## Part B. Writing to the LCD
 
**a. What voltage level do you need to power your display?**

I need 5V to power the display

**b. What voltage level do you need to power the display backlight?**

I also need 5V for the backlight
   
**c. What was one mistake you made when wiring up the display? How did you fix it?**

I tried to connect the GND to the ground and instead connected the pin next to it to the ground. I fixed simply by noticing something's doesn't seem right and changing it. 

**d. What line of code do you need to change to make it flash your name instead of "Hello World"?**

I changed lcd.print("Hello, World!"); to - lcd.print("Tal Genkin");
 
**e. Include a copy of your Lowly Multimeter code in your lab write-up.**

// include the library code:
#include <LiquidCrystal.h>

// initialize the library by associating any needed LCD interface pin
// with the arduino pin number it is connected to
const int rs = 12, en = 11, d4 = 5, d5 = 4, d6 = 3, d7 = 2;
LiquidCrystal lcd(rs, en, d4, d5, d6, d7);

void setup() {
  // set up the LCD's number of columns and rows:
  lcd.begin(16, 2);
  // Print a message to the LCD.
  lcd.print("Tal Genkin");
}

void loop() {
  // Turn off the display:
  lcd.noDisplay();
  delay(500);
  // Turn on the display:
  lcd.display();
  delay(500);
}

## Part C. Using a time-based digital sensor

**Upload a video of your working rotary encoder here.**


## Part D. Make your Arduino sing!

**a. How would you change the code to make the song play twice as fast?**
 
**b. What song is playing?**


## Part E. Make your own timer

**a. Make a short video showing how your timer works, and what happens when time is up!**

https://youtu.be/jLgW4pOovbU

**b. Post a link to the completed lab report your class hub GitHub repo.**
