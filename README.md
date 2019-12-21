# Java-Greenfoot-Cheat-Sheet
This repo has all the function combination for java greenfoot.

Suppose in the project, I have "playerX" as actor and "Game" as world.

## 1. Move the actor
move(NumberofSteps);

Example: 
```move(5);```

## 2. Turn the actor
turn(NumberofDegrees);

Example: 
```python turn(45);```

## 3 Collision Detection.

Suppose playerX is colliding with playerY. Put the following code in playerX editor.

```
Actor collision= getOneIntersectingObject(playerY.class);

if(collision !=null){

    //Do anything here
}
```
## 4. Remove the actor from the world.
```
removeObject(playerX.class);
```
## 5. Add the actor 
```
addObject(playerX.class);
```
## 6. If actor touch the edge, turn it with random angle between 0 and 10.
```
if (isAtEdge())
	{
		turn(Greenfoot.getRandomNumber(10));
	}
  ```  
 ## 7. Resize the image of actor.
 ```
 public class_name()
{
   GreenfootImage image=getImage();
   image.scale(100,100);
   setImage(image);
 }
 ```
 ## 8. Set the Location of the actor.
```
setLocation(Xposition,Yposition);
```
## 9. Set up the world at the beginning.
```
public MyWorld()
    {    
        // Create a new world with 600x400 cells with a cell size of 1x1 pixels.
        super(600, 400, 1); 
        prepare();
    }
//Create the function prepare
private void prepare(){
    addObject(new playerX(),put_Xposition,put_YPosition);
    //Adding object/actor at random position 
    int xrandom=Greenfoot.getRandomNumber(getWidth());
    int yrandom=Greenfoot.getRandomNumber(getHeight());
    addObject(new playerY(),xrandom,yrandom);
    }
```
## 10. Generating random number in Greenfoot.
```
int xrandom=Greenfoot.getRandomNumber(10);//any random value from 0 to 9
```
