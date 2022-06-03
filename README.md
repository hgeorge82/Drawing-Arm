
# SCARA Drawing-Arm

[Planning Doc](https://docs.google.com/document/d/13lnMmdcYeAJbSnfNuPvhkwxSMNHf0qwHTNE0D3j-VtA/edit?scrlybrkr=b64f7e89) 

[Plannig Doc2](https://docs.google.com/document/d/1MwR5_72Ead33QBmqT0MzvE6zn0iQCVVRf9_fdk6CliI/edit)


## Table of Contents
* [Goal](https://github.com/hgeorge82/Drawing-Arm#goal)
* [Supplies](https://github.com/hgeorge82/Drawing-Arm#supplies)
* [Milestones](https://github.com/hgeorge82/Drawing-Arm#milestones)
* [Final Design](https://github.com/hgeorge82/Drawing-Arm#final-design)
* [Problems](https://github.com/hgeorge82/Drawing-Arm/blob/main/README.md#problems)

## Old Goal
To make a SCARA drawing arm that will draw an image, specifically the sigma lab logo. ![Sigma logo](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/Chs%20sigmalogo.png)

## Supplies 
- 2 stepper motors
- A servo 
- Acrylic 3mm
- 3D printed parts
- Arduino
- Arduino CNC shield
- Stepper motor driver board
- GRBL repository

## Milestones
- Plan and research code 

We realized coding this was going to be hard, so with a lot of research we found a GRBL repo that does all the work for us. G-code is the code that's compatible with a SCARA arm. The code was a bit tricky to control on our own so we found a GRBL repository which led to using G code.![UGcode](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/UGScreenshot.png) ![GRBL repository](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/grbl%20screenshot.png)

This is the universal G code and the GRBL repo. Following the instructions with this link 
[GRBL instructions](https://howtomechatronics.com/tutorials/how-to-setup-grbl-control-cnc-machine-with-arduino) it was pretty simple to understand. The universal G code takes the GRBL and transfers it, so instead of drawing lines, it draws an image. Using the X and Y coordinates the drawing utensil can go to any part of the paper. This is basically the "code" we needed for the stepper motors to work. The "code" is just the GRBL being installed onto Arduino. 

![GRBL SCARA on Arduino](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/grbl%20.png) 



- Prototype/plan arm

[Onshape Link](https://cvilleschools.onshape.com/documents/90eec8ce9347071a23da6ff8/w/5e25fa67b4affd436208f593/e/c3920ec5b868799cd839cf0a)

![Gif](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/SM.gif) 

The design started off as an exact copy of another arm, but materials were limited and plans didn't work out. Eventually, we made an easier version as shown in the picture above. This version has two pieces of acrylic with one stepper motor on one of them. 

- Stepper Motor wiring 

The stepper motor has 4 colored wires Green, Yellow, Red, and Gray. The CNC shield there has A1/A2 pins and B1/B2 pins. Red goes to A2 and Yellow goes to A1 while Grey goes to B2 and Green goes to B1. Along with that are 2 driver pinouts that control the pins.
[Wiring](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/Wiring.png)![Wiring](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/Up%20close%20wiring.png)

- Design arm

The arm will be controlled using two stepper motors. Either a servo on the end of the arm to control the writing utensil, or have the arm on a liftable base to reduce weight on the arm. The drawing part of the arm will be connected with a gear and will be moved with belts. One stepper motor has a connectable piece to the first layer of the arm. On the other segment, a stepper motor is placed using a stepper motor mount. The two layers are connected using standoffs. The actual drawing part is connected using an mm gear and a belt. At the end of that drawing part, there's a servo attached which will control the drawing utensil. 

## Problems we encountered 

GRBL SCARA was not working with UGS. Only regular GRBL was compatible with the UGS and that's not what we needed. To try and fix this problem we tried switching computers to see if the computer was the problem, it wasn't. Next, we tried to switch the Arduino board underneath the CNC shield, that also didn't work. Next, we tried using a different version of GRBL, that also didn't work. After many attempts to fix this problem, it still kept showing an "Alarm" on the UGS screen. This problem did not get resolved before the deadline. Measurements were off on our 3D printed parts. Our 3D printed parts were not measured properly and some of the holes were off. To fix this problem we used a file to file the hole open and make it fit. *Don't measure with a ruler to get an exact measurement, use a calibrator* We encountered problems with the range of motion and unequal weight distribution on the arm, so we changed the design. Instead of using a worm, we decided to use a gear with a belt.

![Code](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/CodeScreenshot1.png)


## New Goal
Make a scara drawing arm that will draw anything(probaby a line) the user wants with potentiometers.

## New Changes 
We changed the way the stepper motors are controlled. Our original idea was to use GRBL SCARA and UGS to control the stepper motors. There was something that just wasn't working and we couldn't find anything that could solve our problem. Instead, we decided to control the stepper motors with potentionemters like an Etch-A-sketch. Most of the design intent samed the same, like the box, the steppermotor parts, and the servo parts. 


New Code
![Code](https://github.com/hgeorge82/Drawing-Arm/blob/main/images/CodeScreenshot1.png)

## Final Design
The arm is controlled by using two potentiometers. Like an Etch-A-Sketch it will draw anything that the user wants to draw if they turn the potentiometers. The arm part consists of a steeper motor inside the box. The stepper motor is mounted to fit using a stepper holder. On top of that steppermotor is an adapter. On top of that adapter is the arm. The arm consists of to bases connected together with the use of brackets. The actual arm part that will draw is connected with a gear and a belt. At the end of the arm there is a servo with a servo holder/mount thing.

## Reflection

























