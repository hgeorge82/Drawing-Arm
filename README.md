# Scara Drawing-Arm

## Goal
To make a Scara drawing arm that will draw an image, specifically the sigma lab logo. 

## Supplies needed
- 2 stepper motors
- A servo 
- Arcylic 3mm
- 3D printed part...
- Arduino
- Arduino cnc shield
- Stepper motor driver board
- grbl repository
- Worm screw?

## Milestones
Plan and research code
- Realized coding this was going to be hard so, using a scara arm arduino code guideline we found an outline that does the coding for us. G-code is the code that's compatible with a scara arm.
Proper prototype
Get the stepper motors to move
Import a g-code file for the arm to draw
Command the arm to move using g-code
Having an arm that moves with a sturdy base/arm
Having the arm move with g-code coordinates converted to polar coordinates
Finalize code

Description

The arm will be controlled using two stepper motors. Either a servo on the end of the arm to control the writing utensil, or have the arm on a liftable base to reduce weight on the arm. The drawing part of the arm will be connected with a gear and will be moved with belts. On top of one of the stepper motors it starts of with a 3D printed piece sandwiched between two rings. On top of those rings starts the arm. The arm consists of two piece arcylic conncted with bolts. On top of those pieces is a stepper motor place previously where the other one is. Also the drawing arm piece that's connected by a gear and will be moved with belts. 135mm drawing piece, 135mm arm parts, 45mm diameter ring, 31.831mm diameter gears, 12.7mm apart are the two pieces. It will mainly be made up of arcylic with the addition of some 3d printed parts.

![grbl screenshot](https://user-images.githubusercontent.com/71407017/149539549-78858c83-d3bb-411f-9aa4-52939c9474c7.png)
![Example 1](https://user-images.githubusercontent.com/71407017/149539760-bfa3f358-26f1-4adc-9907-9906ecca15b4.png) 
![Example 2](https://user-images.githubusercontent.com/71407017/149539886-1a7be6fc-a0eb-424a-a88b-248c7c801427.png)
![Example 3](https://user-images.githubusercontent.com/71407017/149539899-7c9a35a5-f28f-4c80-ae3b-012cc656271f.png) 
![Rough Sketch](https://user-images.githubusercontent.com/71407017/149540030-b95e0377-2394-430b-90cd-200b2f863f92.png)


