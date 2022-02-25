# Scara Drawing-Arm

## Table of Contents
* [Goal](https://github.com/hgeorge82/Drawing-Arm#goal)
* [Supplies](https://github.com/hgeorge82/Drawing-Arm#supplies)
* [Milestones](https://github.com/hgeorge82/Drawing-Arm#milestones)
* [Final Design](https://github.com/hgeorge82/Drawing-Arm#final-design)
* [Problems](https://github.com/hgeorge82/Drawing-Arm/blob/main/README.md#problems)

## Goal
To make a Scara drawing arm that will draw an image, specifically the sigma lab logo. ![Sigma logo](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/Chs%20sigmalogo.png)

## Supplies 
- 2 stepper motors
- A servo 
- Arcylic 3mm
- 3D printed part...
- Arduino
- Arduino cnc shield
- Stepper motor driver board
- grbl repository

## Milestones
- Plan and research code (Import g code, a small sketch to help)
Realized coding this was going to be hard, so using a grbl repository, we found an outline that does the coding for us. G-code is the code that's compatible with a scara arm. The code was a bit tricky to control on our own so we found a grbl repository which led to using G code.![UGcode](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/UGScreenshot.png) ![gbrl repository](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/grbl%20screenshot.png) This is the universal G code, using this code we input the stepper motor code which basically does all the work for us. The universal G code takes the setpper motor code and transfers it, so instead of drawing lines it draws an image. Using the X and Y coordinates the drawing utensil can go to any part of the paper. This is basically the "code" we needed for the stepper motors to work. The "code" is just the grbl being installed onto arduino.

![grbl scara on arduino](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/grbl%20.png) 


- Prototype/plan arm
[Onshape Link](https://cvilleschools.onshape.com/documents/90eec8ce9347071a23da6ff8/w/5e25fa67b4affd436208f593/e/c3920ec5b868799cd839cf0a)
![Gif](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/SM.gif) 

The design started of as an exact copy of another arm, but materials were limited and plans didn't work out. Eventually we made an easier version as shown in the picture above. This version has two pieces of arcylic with one stepper motor on one of them. 

- Stepper Motor wiring 
There are 4 colored wires, Green, Yellow, Red, and Gray and on the CNC shield there are A1/A2 pins and B1/B2 pins. Red goes to A2 and Yellow goes to A1 while Grey goes to B2 and Green goes to B1
[Wiring](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/Wiring.png)![Wiring](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/Up%20close%20wiring.png)

- Design arm
The arm will be controlled using two stepper motors. Either a servo on the end of the arm to control the writing utensil, or have the arm on a liftable base to reduce weight on the arm. The drawing part of the arm will be connected with a gear and will be moved with belts. One stepper motor has a connetable piece to the first layer of the arm. On the other segment a stepper motor is placed using a mount. The two layers are connected using standoffs. The actual drawing part is connected using a mm gear and a belt. On the end of that drawing part thers'a a servo attached which will control the drawing utensil. 

## Final Design

The arm is controlled by using stepper motors. Either a servo on the end of the arm to control the writing utensil or have the arm on a liftable base to reduce weight on the arm. One arm segment will be conncted to a stepper motor using an adapter. The other arm segment will have a stepper mount to connect the stepper motor. Those two segments will be held together using standoffs. The drawing segment has a servo on the end with a servo mount, connected with a mm gear and a belt.
![Final Design](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/Final.png)  


## Problems we encountered 

Grbl scara was not working with UGS. In order for the stepper motors to work we needed the UGS and grbl scara. Only regular grbl was compatible with the UGS and that's not what we needed. To overcome this problem we tried switching computers to see if the computer was the problem, it wasn't. Next we tried to switch the arduino board underneath the CNC shield, that also didn't work. Next we tried using a different. Measurements were of on our 3D printed parts. Our 3D printed parts were not meausured properly and some of the holes were off. To fix this problem we used a file to file the hole open and make it fit. *Don't meausre with a ruler to get an exact measurement, use a calibrator.* We struggled with this because our original design was going to make the motion harder to do.  So to fix this decided to change our design and use belts to move the drawing piece. 
As said before our design made the motion complicated as well as an unequal distribution of weight and we didn't want the arm to tilt any more than it has too. 

























