# Java-Greenfoot-Cheat-Sheet
This repo has all the function combination for java greenfoot.

Suppose in the project, I have playerX as actor and Game as world.

## 1. Move the actor
move(NumberofSteps);

Example: move(5);

## 2. Turn the actor
turn(NumberofDegrees);

Example: turn(45);

## 3: Collision Detection
''' Suppose playerX is colliding with playerY. Put the following code in playerX editor.

Actor collision= getOneIntersectingObject(playerY.class);

if(collision !=null){

    //Do anything here
    
} '''
