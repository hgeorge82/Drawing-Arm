# SCARA Drawing-Arm

## Table of Contents
* [Goal](https://github.com/hgeorge82/Drawing-Arm#goal)
* [Supplies](https://github.com/hgeorge82/Drawing-Arm#supplies)
* [Milestones](https://github.com/hgeorge82/Drawing-Arm#milestones)
* [Final Design](https://github.com/hgeorge82/Drawing-Arm#final-design)
* [Problems](https://github.com/hgeorge82/Drawing-Arm/blob/main/README.md#problems)

## Goal
To make a SCARA drawing arm that will draw an image, specifically the sigma lab logo. ![Sigma logo](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/Chs%20sigmalogo.png)

## Supplies 
- 2 stepper motors
- A servo 
- Arcylic 3mm
- 3D printed part...
- Arduino
- Arduino cnc shield
- Stepper motor driver board
- GRBL repository

## Milestones
- Plan and research code (Import g code, a small sketch to help)
Realized coding this was going to be hard, so using a GRBL repository, we found an outline that does the coding for us. G-code is the code that's compatible with a SCARA arm. The code was a bit tricky to control on our own so we found a GRBL repository which led to using G code.![UGcode](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/UGScreenshot.png) ![GRBL repository](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/grbl%20screenshot.png) This is the universal G code, using this code we input the stepper motor code which basically does all the work for us. The universal G code takes the stepper motor code and transfers it, so instead of drawing lines it draws an image. Using the X and Y coordinates the drawing utensil can go to any part of the paper. This is basically the "code" we needed for the stepper motors to work. The "code" is just the GRBL being installed onto Arduino. ![GRBL SCARA on Arduino](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/grbl%20.png) 

-  Using GRBL with a cnc shield
[GRBL instructions](https://howtomechatronics.com/tutorials/how-to-setup-grbl-control-cnc-machine-with-arduino/)
- download GRBL firmware from github
- open it and download as a zip 
- open and extract the zip file
- sketch, include library, add zip library
- Open the GRBL master file, then open the GRBL file
- file, examples, GRBL, GRBL upload 

- Prototype/plan arm
[Onshape Link](https://cvilleschools.onshape.com/documents/90eec8ce9347071a23da6ff8/w/5e25fa67b4affd436208f593/e/c3920ec5b868799cd839cf0a)
![Gif](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/SM.gif) 

The design started of as an exact copy of another arm, but materials were limited and plans didn't work out. Eventually we made an easier version as shown in the picture above. This version has two pieces of arcylic with one stepper motor on one of them. 

- Stepper Motor wiring 
The stepper motor has 4 colored wires Green, Yellow, Red, and Gray. The CNC shield there has A1/A2 pins and B1/B2 pins. Red goes to A2 and Yellow goes to A1 while Grey goes to B2 and Green goes to B1. Along with that there are these things called 
[Wiring](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/Wiring.png)![Wiring](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/Up%20close%20wiring.png)

- Design arm
The arm will be controlled using two stepper motors. Either a servo on the end of the arm to control the writing utensil, or have the arm on a liftable base to reduce weight on the arm. The drawing part of the arm will be connected with a gear and will be moved with belts. One stepper motor has a connetable piece to the first layer of the arm. On the other segment a stepper motor is placed using a mount. The two layers are connected using standoffs. The actual drawing part is connected using a mm gear and a belt. On the end of that drawing part thers'a a servo attached which will control the drawing utensil. 

## Final Design

![Final Design](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/Final.png)  
![]()
![]()

## Problems we encountered 

GRBL SCARA was not working with UGS. Only regular GRBL was compatible with the UGS and that's not what we needed. To try and fix this problem we tried switching computers to see if the computer was the problem, it wasn't. Next we tried to switch the arduino board underneath the CNC shield, that also didn't work. Next we tried using a different version of grbl, that also didn't work. After many attempts fix this problem it still kept showing an "Alarm." This problem did not get resolved before the deadline. Measurements were off on our 3D printed parts. Our 3D printed parts were not meausured properly and some of the holes were off. To fix this problem we used a file to file the hole open and make it fit. *Don't meausre with a ruler to get an exact measurement, use a calibrator* We encountered problems with the range of motion and an unequal weight distribution on the arm, so we changed the design. Instead of using a worm we decied to use a gear with a belt.


























