# Use the light sensor in an Adafruit Circuit Playground as an input device in a Processing program
In this Arduino lab you will write a program that gets input from the light sensor in the [Adafruit Circuit Playground](https://www.adafruit.com/product/3000) and uses it as an controller so that you can interact with your Virtual Pet from the [previous assignment](https://github.com/APCSLowell/VirtualPet/blob/gh-pages/README.md#virtual-pet).

### Step 1: Plug in the Adafruit Circuit Playground and start Processing
Connect the Circuit Playground to your computer with a USB cord. Open Processing. You will need to install a library (you only need to do this once). Choose *Sketch | Import Library | Add Library*.  Type *Arduino* in the text field labeled *Filter*. Choose *Arduino (Firmata)* and click *Install*.

### Step 2: Run this sample program
Copy and paste the following program
```java {.line-numbers}
import processing.serial.*;
import cc.arduino.*;
Arduino arduino;

public void setup() {
  size(500, 500);
  arduino = new Arduino(this, Arduino.list()[0], 57600); //change the [0] to a [1] or [2] etc. if your program doesn't work
}

public void draw() {
  background(192);
  int y = arduino.analogRead(5);
  System.out.println(y);
  ellipse(250, 2*y, 50, 50);
}
```
Run the program. Pass your hand over the light sensor labeled with a picture of an eye on the Circuit Playground. You should see an ellipse move up and down as the light sensor changes values. Higher values mean more light. The light sensor is circled in the picture below. On some machines, you may need to change the last line in `setup()` to get the program to work correctly.
![](CircuitPlayground.PNG)

### Step 3: Write your own program
Using the sample program as a guide, write your own program that uses the light sensor. Your program doesn't have to work or look like any other. Have fun and be creative! 

### Step 4: Make a short video (under 10 seconds and smaller than 25MB)
When you are happy with your program, have a friend make a short video of you interacting with your virtual pet. The video need only show your hand, the arduino and your pet, please don't include anyone's face in the video. See Mr. Simon's example animated gif and the samples of student work below.   

Convert the video to an animated gif using a free converter like [ezgif.com](https://ezgif.com/). Use ezgif's *cut video* or a similar option to edit your video to under 10 seconds and less than 25MB. Upload your animated gif to your VirtualPet repository. Submit the link to your gif to Google Classroom. 

[Mr. Simon's virtual pet penguin animated gif](VirtualPenguin.gif)   

<!-- ### Have something cool that can be shown at back to school night?
Back to school night is Thursday September 19. Let me know if I can use your program at back to school night.   -->

Samples of Student Work
-----------------------
[Keneth](https://github.com/KenethL/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Kaitlyn](https://github.com/kaiyenpepper/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Federico](https://github.com/feaprile/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Viva](https://github.com/vivavoong/VirtualPet/blob/gh-pages/interactingwithfish.gif)   
[Chris](https://github.com/TophTheBro/LightSensorController/blob/master/ezgif.com-video-to-gif.gif)   
[Tiffany](https://github.com/TILOUIE2/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Jimmy](https://github.com/Jimmy1433223/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Sam](https://github.com/SamRosenblum415/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Albert](https://github.com/alshi31/VirtualPet/blob/gh-pages/Albert%20Shi's%20Virtual%20Pet%20Panda%20GIF.gif)   
[Michelle](https://github.com/mitan4/VirtualPet/blob/gh-pages/birdHop.gif)   
[Alison](https://github.com/apcsci/VirtualPet/blob/gh-pages/virtualpet_gif.gif)   
[Nikhita](https://github.com/Nilaw5/VirtualPet/blob/gh-pages/VirtualPet%20Light%20Gif.gif)   
[Eric](https://github.com/erchan3/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Chun Ho](https://github.com/chchen4/VirtualPet/blob/gh-pages/Mad%20Virtual%20Pet.gif)   
[Jocelyn](https://github.com/jxcelynyu/VirtualPet/blob/gh-pages/IMG_0589.GIF)   
[Zoey](https://github.com/zoeyzhu/VirtualPet/blob/gh-pages/IMG_8305.GIF)   
[Tyler](https://github.com/ty237/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Tiffany](https://github.com/tiffanyt11/VirtualPet/blob/gh-pages/ezgif-7-49449e974dc8.gif)   
[Alex](https://github.com/AlexHackathon/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Max](https://github.com/max-2023/VirtualPet/blob/gh-pages/Maxwell%20Xu%20-%20Interactive%20Virtual%20Pet.gif)   


weeeeeeee
[Bruno](https://github.com/bruno-415/VirtualPet/blob/gh-pages/petoctopus_gif.gif)   
[Damian](https://github.com/dabogdon/LightSensorController/blob/master/ezgif-7-c98aa93edc26.gif)    
[Alvin](https://github.com/alchan6/VirtualPet/blob/gh-pages/Virtual%20Pet%20Gif.gif)    
[Wing](https://github.com/wilai3/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(1).gif)    
[Aiden](https://github.com/AidenShiu/VirtualPet/blob/gh-pages/ezgif-7-ab505aa2b4a4.gif)   
[Andrew](https://github.com/antan2/VirtualPet/blob/gh-pages/light%20sensor%20gif.gif)   
[William](https://github.com/wicao1/VirtualPet/blob/gh-pages/virtual_pet_gif.gif)   
[Chris](https://github.com/ChGee/VirtualPet/blob/gh-pages/D1A03D0F-BAB3-42A9-9C4A-906D4511673D.gif)   
[Kumiko](https://github.com/kukomori/VirtualPet/blob/b213ec85dfabac02a42f1126524f14b71b459cdd/doggy.gif)    
[Karina](https://github.com/kaanders17/VirtualPet/blob/gh-pages/Virtual%20Pet%20GIF.gif)  
[Paolo](https://github.com/paolo415/VirtualPet/blob/gh-pages/lightSensorShark.gif)  
[Breanna](https://github.com/paolo415/VirtualPet/blob/gh-pages/lightSensorShark.gif)  
[Edward](https://github.com/edpilotte/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif) 
[Jeffrey](https://github.com/edpilotte/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)  
[Austin](https://github.com/auwong1/VirtualPet/blob/908332eadb26acada225312c10647b8ef24e5854/bear.gif)  
[Jason](https://github.com/jawong32/Virtual-Pet-Animation)  
