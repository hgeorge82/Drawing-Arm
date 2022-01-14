# Scara Drawing-Arm

## Problem
To make a Scara drawing arm that will draw an image, specifically the sigma lab logo. 

## Supplies needed
-2 stepper motors
-A servo 
-Arcylic 3mm
-3d printed part...
-Arduino
-Arduino cnc shield
-Stepper motor driver board
-grbl repository

## Milestones?
Plan and research code
- 
Write code and prototype
- G-code is the code that's compatible with as scara arm. The problwm is it would be hard to code through arduino, so in order to make it easier use a grbl respositry that will do everything for us. 
-  import a g-code file for the arm to draw![grbl screenshot](https://user-images.githubusercontent.com/71407017/149539549-78858c83-d3bb-411f-9aa4-52939c9474c7.png)
-  command the arm to move using g-code

https://github.com/jared-hughes/grbl-scara
Prototype/plan arm
A proper design 
 It will mainly be made up of arcylic and an extra 3d printed piece. The base of the arm is simply a box with the diimensions of 127 W 127 L and H 50.8mm. The design is still a work in progress but orignally it was going to model Example 3. However, the base would different and more of a boxy shape. There are 3 examples we're going off of and from these 3 examples we combined them and created a rough sketch of what would it would look like. Our plan originally was to use servos to control the arms movement, but soon realiized it would be a problem. Stepper motors would control the arms movement way better. Either a servo on the end of the arm to control the writing utensil, or have the arm on a liftable base to reduce weight on the arm. 
 - length of arms
 - belts?
 - Worm screw?

![Example 1](https://user-images.githubusercontent.com/71407017/149539760-bfa3f358-26f1-4adc-9907-9906ecca15b4.png)
![Example2](https://user-images.githubusercontent.com/71407017/149539886-1a7be6fc-a0eb-424a-a88b-248c7c801427.png)
![Example](https://user-images.githubusercontent.com/71407017/149539899-7c9a35a5-f28f-4c80-ae3b-012cc656271f.png)
![Rough Sketch](https://user-images.githubusercontent.com/71407017/149540030-b95e0377-2394-430b-90cd-200b2f863f92.png)


Having an arm that moves with a sturdy base/arm
- Have yet to make actual arm or prototype
Having the arm move with g-code coordinates converted to polar coordinates
- tbd
Finalize code
- tbd






