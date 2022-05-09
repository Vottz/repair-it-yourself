# RIY - Repair it yourself
This is the Documentation for our university project, in the course [Hacking Innovation Bias](https://moseskonto.tu-berlin.de/moses/modultransfersystem/bolognamodule/beschreibung/anzeigen.html;jsessionid=ObAu5fcd4ZbIFyQYRfJkT4t84GxhwX-60i1GFf0u.moseskonto?nummer=50836&version=3&sprache=1) at the Technical University of Berlin.




## Functions
Our Arduino code has 3 Functions: 
* setup(): the typical arduino setup function, here we define the randomSeed for the random number generator, the <LCDs groove text> matrix for setting the display functions and some of the LED lights <DO WE??>.
* calcRangeInCentimeters(): calculates the distance from the <INSERT NAME OF SENSOR + LINK> in centimeters
* randomText(int randNum): with the input of a random number between 0 and 6, one of the critical texts is returned
* loop(): the typical arduino "main" function, that gets executed repeatedly. Here we use the previous two functions, as explained above.
In each iteration, we generate a random number for the randomText() function and then assign a color to that text (specifying the gender-role we are critisizign with that text). Then the calcRangeInCentimeters() function is used to determine if something is 20cm in front of the sensor, if yes the text and color are displayed on the <LCD GROOVE LIGHT????> and the LEDs light up. We implemented a 3second delay which should be enough time for the observer to read the text. 

## Contributors
Kevin Kreutz  
Dina Schaltuganow  
Tabea Claudia Zeltner
