# RIY - Repair it yourself
This is the Documentation for our university project, in the course [Hacking Innovation Bias](https://moseskonto.tu-berlin.de/moses/modultransfersystem/bolognamodule/beschreibung/anzeigen.html;jsessionid=ObAu5fcd4ZbIFyQYRfJkT4t84GxhwX-60i1GFf0u.moseskonto?nummer=50836&version=3&sprache=1) at the Technical University of Berlin.

[Final presentation](/RIY.pdf), with project summary, background information and more pictures


## Arduino setup
<ToDo>


## Functions
Our Arduino code has 4 Functions: 
* setup(): the typical arduino setup function, here we define the randomSeed for the random number generator, the <LCDs groove text> matrix for setting the display functions and some of the LED lights.
* calcRangeInCentimeters(): calculates the distance wth help of the [Ultrasonic-Sensor-sr04](https://create.arduino.cc/projecthub/abdularbi17/ultrasonic-sensor-hc-sr04-with-arduino-tutorial-327ff6) in centimeters
* randomText(int randNum): with the input of a random number between 0 and 6, one of the critical texts is returned
* loop(): the typical arduino "main" function, that gets executed repeatedly. Here we use the previous two functions, as explained above.
In each iteration, we generate a random number for the randomText() function and then assign a color to that text (specifying the gender-role we are critisizign with that text). Then the calcRangeInCentimeters() function is used to determine if something is 20cm in front of the sensor, if yes the text and color are displayed on the [Grove-LCD RGB Backlight](https://wiki.seeedstudio.com/Grove-LCD_RGB_Backlight/) and the LEDs light up. We implemented a 3 second delay which should be enough time for the observer to read the text. 

## Resources used
### Libraries
* <Wire.h>
* "rgb_lcd.h"
* "Ultrasonic.h"
### Documentation
* [Ultrasonic Ranger (wiki.seedstudio.com)](https://wiki.seeedstudio.com/Grove-Ultrasonic_Ranger/)
* [LED circuit (arduino.cc)](https://create.arduino.cc/projecthub/rowan07/make-a-simple-led-circuit-ce8308)
* [LCD display(arduino.cc)](https://docs.arduino.cc/learn/electronics/lcd-displays)
* And many thanks to [Carolin Clausnitzer](https://www.technologiestiftung-berlin.de/profil/team/carolin-clausnitzer) & [Ninett Rosenfeld](https://www.technologiestiftung-berlin.de/profil/team/ninett-rosenfeld) from the [Technologiestiftung Berlin](https://www.technologiestiftung-berlin.de/), who provided us with the basics and initial functions in their "Digital Workshop Creative Making mit Arduinos". Additionally we would like to thank the [Technologiestiftung Berlin](https://www.technologiestiftung-berlin.de/) in general for lending us the Arduinos, which made this artefact possible.

## Contributors
Kevin Kreutz  
Dina Schaltuganow  
Tabea Claudia Zeltner
