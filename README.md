# Use an Adafruit Circuit Playground as an input device in a Processing program
In this Arduino lab you will write a program that gets input from the light sensor in the Adafruit Circuit Playground and use it as an controller for a Processing program

### Step 1: Plug in the Adafruit Circuit Playground and start Processing
Contact the Circuit Playground to your computer with a USB cord. Open Processing. You will need to install a library (you only need to do this once). Choose *Sketch | Import Library | Add Library*.  Type *Arduino* in the text field labeled *Filter*. Choose *Arduino (Firmata)* and click *Install*.

### Step 2: Run this sample program
Copy and paste the following program
```java {.line-numbers}
import processing.serial.*;
import cc.arduino.*;
Arduino arduino;

void setup() {
  size(500, 500);
 arduino = new Arduino(this, Arduino.list()[0], 57600);
  
  // Set the Arduino digital pins as inputs.
  for (int i = 0; i <= 13; i++)
    arduino.pinMode(i, Arduino.INPUT);
}

void draw() {
    background(192);
    int y = arduino.analogRead(5);
    ellipse(250,2*y,50,50);
}
```


### Step 3: 
TBD

### Extensions:
TBD
