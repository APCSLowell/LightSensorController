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
When you are happy with your program, have a friend make a short video of you interacting with your virtual pet. The video need only show your hand, the arduino and your pet, please don't include anyone's face in the video. See the samples of student work below.   

Convert the video to an animated gif using a free converter like [ezgif.com](https://ezgif.com/). Use ezgif's *cut video* or a similar option to edit your video to under 10 seconds and less than 25MB. Upload your animated gif to your VirtualPet repository. Submit the link to your gif in Google Classroom. 

<!-- ### Have something cool that can be shown at back to school night?
Back to school night is Thursday September 19. Let me know if I can use your program at back to school night.   -->

Samples of Student Work
-----------------------
[Sean](https://github.com/GeraldJimes/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Curtis](https://github.com/curtischen1/VirtualPet/blob/gh-pages/LightSensor.gif)   
[Kenny](https://github.com/KennyCh13/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Cameron](https://github.com/CaNguyen1/VirtualPet/blob/gh-pages/IMG_6046.GIF)   
[Pansy](https://github.com/pakuang/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Nash](https://github.com/MoonNash/VirtualPet/blob/gh-pages/IMG_2826%20(1).GIF)   
[Koey](https://github.com/koeychan/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Leah](https://github.com/Lloyd2202/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Mikey](https://github.com/miosullivan/LightSensorController/blob/master/ezgif.com-gif-maker.gif)   
[Jonah](https://github.com/JonahWaldman/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Gabriella](https://github.com/gabriellasu/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(1).gif)   
[Keneth](https://github.com/KenethL/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Johnny](https://github.com/Jlin202/VirtualPet/blob/gh-pages/ezgif-2-10cdb474aac4.gif)   
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
[Jeffrey](https://github.com/jethiDaCoder/VirtualPet/blob/gh-pages/Virtual%20Pet%20Pufferfish.gif)    
[Austin](https://github.com/auwong1/VirtualPet/blob/908332eadb26acada225312c10647b8ef24e5854/bear.gif)  
[Jason](https://github.com/jawong32/Virtual-Pet-Animation/blob/main/arduino.gif)  
[Haden](https://github.com/hachan-beep/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(1).gif)    
[Irisa](https://github.com/irisac415/VirtualPet/blob/gh-pages/Light%20Sensor%20Snowman%20Gif.gif)   
[Matthew](https://github.com/malee8/VirtualPet/blob/gh-pages/Light%20Sensor%20(Aug%2031%2C%202021%20at%208_08%20AM).gif)    
[Luke](https://github.com/LukeD808/VirtualPet/blob/gh-pages/LukeDonohueVirtualPetGif.gif)   
[Hayden](https://github.com/hakwok/VirtualPet/blob/gh-pages/gif.gif)    
[Noella](https://github.com/noellalee1/VirtualPet/blob/gh-pages/63DEBE89-4BAA-44AE-8227-19408460A609.gif)   
[Eric](https://github.com/ErLiao137/VirtualPet/blob/gh-pages/owl_gif2.gif)   
[Joyce](https://github.com/joliu8/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Vivian](https://github.com/VivianMak/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Lexian](https://github.com/lexiannguyen/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)    
[Nathan](https://github.com/NathanTjong/VirtualPet/blob/gh-pages/D29BD7F0-F638-4114-BDD5-F430A6F304E6.gif)    
[Rafa](https://github.com/IamRafaelllll/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)  
[Nicolas](https://github.com/nireiss/VirtualPet/blob/2dbc2fafb4534644acdb4300800e627c9ff09694/nicolasReissVirtualPetArduino.gif)   
[Christina](https://github.com/christina88chan/VirtualPet/blob/5a5e5561933f2b6075028a15997f6c5555fae52a/bear.GIF)   
[Joanne](https://github.com/joannechenn/LightSensorController/blob/master/ezgif.com-gif-maker.gif)   
[Caitlyn](https://github.com/calam1818/VirtualPet/blob/gh-pages/ezgif-7-2a34deac5c28.gif)   
[Ye](https://github.com/YejinL12/VirtualPet/blob/1e12aa4eacfa27f8f2b6a9adce5fa1f9b545c9c2/speedyOcto.gif)   
[Van](https://github.com/Vanthebot/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Joshua](https://github.com/jopaza21/VirtualPetAnimation/blob/main/VirtualPetLightAnimation1.gif)   
[Justin](https://github.com/jushiu/Animation/blob/main/EC6B3633-1839-4E79-8E68-1988A1A46386.gif)   
[Eric](https://github.com/desolaterakan/VirtualPet/blob/gh-pages/froog-old.gif)   
[Dylan](https://github.com/dy-alt/VirtualPet/blob/gh-pages/elephant.gif)   
[Mira](https://github.com/mira16-v/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%281%29.gif)   
[Ivana](https://github.com/ivxu24/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Gary](https://github.com/Gary055/anime/blob/main/ezgif.com-gif-maker.gif)   
[Emily](https://github.com/emyip/VirtualPet/blob/gh-pages/VID_20210902_083010.gif)   
[Akemi](https://github.com/Akemi1222/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif.gif)   
[William](https://github.com/WilliamsGitHubAccount/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Stephen](https://github.com/stevenmeap/VirtualPet/blob/gh-pages/SnowmanGif.gif)   
[Daniel](https://github.com/wood09/VirtualPet/blob/gh-pages/ezgif-6-a204699bbd88-min.gif)   
[Lilia](https://github.com/liliaching/VirtualPet/blob/944e4f1785dd7701158b9dc16cd2ad84d9d05429/B49FD15F-75E7-413A-9D82-B061CC1A6359.gif)   
[Andrew](https://github.com/guppies23456/LightSensorController/blob/master/AD%20Light%20Sensor%20Virtual%20Pet.gif)   
[Luke](https://github.com/LukeD808/VirtualPet/blob/gh-pages/LukeDonohueVirtualPetGif.gif)   
[Liam](https://github.com/ligiraldo/VirtualPet/blob/gh-pages/beanospoke.gif)   
[Hayden](https://github.com/hakwok/VirtualPet/blob/gh-pages/gif-min.gif)   
[Jacob](https://github.com/jalambert/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Noella](https://github.com/noellalee1/VirtualPet/blob/gh-pages/63DEBE89-4BAA-44AE-8227-19408460A609.gif)   
[Eric](https://github.com/ErLiao137/VirtualPet/blob/gh-pages/owl_gif2.gif)   
[Joyce](https://github.com/joliu8/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Vivian](https://github.com/VivianMak/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Lexian](https://github.com/lexiannguyen/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Rafael](https://github.com/IamRafaelllll/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Nathaniel](https://github.com/NathanTjong/VirtualPet/blob/gh-pages/D29BD7F0-F638-4114-BDD5-F430A6F304E6.gif)   
[Nicolas](https://github.com/nireiss/VirtualPet/blob/2dbc2fafb4534644acdb4300800e627c9ff09694/nicolasReissVirtualPetArduino.gif)   
[Brian](https://github.com/brsen/VirtualPet/blob/gh-pages/1037EF2E-6A72-49FE-BAED-48B60620A940.gif)   
[Justin](https://github.com/jushiu/Animation/blob/main/EC6B3633-1839-4E79-8E68-1988A1A46386.gif)   
[Stella](https://github.com/StellaSit0/VirtualPet/blob/gh-pages/ezgif-2-2963dcfd78fd.gif)   
[Wendy](https://github.com/lafmj/VirtualPet/blob/gh-pages/sdasdasda.gif)   
[Joseph](https://github.com/JosephTeng/VirtualPet/blob/gh-pages/D2DB5951-7BB4-48D7-84E4-EDB18E421764.gif)   
[Joshua](https://github.com/jovegher/VirtualPet/blob/gh-pages/virtualpetlightsensor.gif)   
[Brianna](https://github.com/brwong8/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif.gif)   
[Justin](https://github.com/Justin-pyth/VirtualPet/blob/gh-pages/Light%20Sensor.gif)   
[Qiao Yan](https://github.com/QIAOYANX/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Caden](https://github.com/cayeung1/VirtualPet/blob/gh-pages/ezgif-2-52c35b7d5a6d.gif)   
[Tommy](https://github.com/toyu3/VirtualPet/blob/gh-pages/ezgif-2-98d14e342430.gif)   
[David](https://github.com/davidzhang3/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Darren](https://github.com/DarrenZhao1/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%204.gif)   
[Hui Shan](https://github.com/huishancai/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif.gif)   
[Brennan](https://github.com/Brennan-c/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Jennifer](https://github.com/jennifer0525/VirtualPet/blob/gh-pages/virtual%20pet%20gif.gif)   
[Deion](https://github.com/deionchaudhary/Panda/blob/gh-pages/lightSensor.gif)   
[Aaron](https://github.com/AaronnChen/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Jackie](https://github.com/jachen16/VirtualPet/blob/gh-pages/Animated%20Pet.gif)   
[Christina](https://github.com/chchung1/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Joselino](https://github.com/joselinodt/VirtualPet/blob/gh-pages/IMG-9425.GIF)   
[Nathan](https://github.com/Naguan1/VirtualPet/blob/6e7fbb24cdc168d90c971d984f71812e4eb09cf9/ezgif.com-gif-maker%20%282%29.gif)   
[Munkhtushie](https://github.com/tushigitgel/VirtualPet/blob/gh-pages/myhippodancinggif.gif)   
[Kyle](https://github.com/kylam1/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Noelle](https://github.com/noellelam/VirtualPet/blob/71284452804fd61c948c9267f2222da075141f3c/ezgif.com-gif-maker.gif)   
[Andy](https://github.com/andeey3/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Audrey](https://github.com/AudreyLau8/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[William](https://github.com/Williamlaw2005/VirtualPet/blob/gh-pages/ezgif-7-cce55bd8754a.gif)   
[Jenna](https://github.com/Jenna1910/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Ryan](https://github.com/chknwngs999/VirtualPet/blob/gh-pages/chickengif.gif)   
[Nathan](https://github.com/naleung1/VirtualPet/blob/gh-pages/Pet%20Slime%20Light%20Sensor%20gif.gif)   
[Ivy](https://github.com/ivyylin/VirtualPet/blob/gh-pages/1B2E0BCA-88D3-49C1-9004-450437B2E30D.gif)   
[Gabriel](https://github.com/Gabriel-Low-06/VirtualPet/blob/157d3f24c5e159068432e7cedebacd9efa10579f/Dragon-LightSensor.gif)   
[Joyce](https://github.com/joycema212/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif.gif)   
[Mika](https://github.com/mikanguyenn/VirtualPet/blob/gh-pages/VirtualPet.gif)   
[Sophia](https://github.com/sophiapeckner/VirtualPet/blob/gh-pages/flappyCardinal.gif)   
[Ethan](https://github.com/Etqiu/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Emeley](https://github.com/emsarcenobravo/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Nate](https://github.com/Nsirival/VirtualPet/blob/gh-pages/Nate%20Sirivallop%20-%20Light%20Sensor.gif)   
[Eric](https://github.com/desolaterakan/VirtualPet/blob/gh-pages/froog-old.gif)   
[Koen](https://github.com/koendwong/VirtualPet/blob/gh-pages/koendwongPandaBounce.gif)   
[Annie](https://github.com/anxu9/VirtualPet/blob/gh-pages/bunnygif.gif)   
[Brayden](https://github.com/B-r-4-y-d-3-n/VirtualPet/blob/gh-pages/ezgif-4-996eba0ef3d6.gif)   
[Jason](https://github.com/JasonZhong3/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%282%29.gif)   
[Ivan](https://github.com/ivzhu1/VirtualPet/blob/gh-pages/duck.gif)   
[Tobias](https://github.com/TobyZuercher/VirtualPet/blob/gh-pages/image0.gif)   
