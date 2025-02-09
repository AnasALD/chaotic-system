# chaos-balls

Balls bouncing inside of a circle. This was inspired by a similar Numberphile video on chaotic systems.

## Requirements

- python 3.9

Using pip install these packages:

- pygame.

```pip install pygame```

- numpy (not sure but get it just in case)

```pip install numpy```

## Run

Simply run the chaos_balls.py file either by double clicking it or

```py chaos_balls.py```

## Features

To Add/Remove balls and manipulate their properties, i.e velocity, position, etc you can do so by opening chaos_balls.py in a text editor and follow the instructions around line 150.

Example:

To add a red ball at the position 200, 300. 

First we will create the object:

```redball_test = Balls()```
Now the arguments that go in the class Balls are seen in the template below:

```template = Balls("name", color, radius, thickness, x-coordinate, y-coordinate, [collision sound file] optional)```

 - name: name of the ball, call it whatever you like -> str
 - color: color of the ball. color is a tuple of the format (r,g,b)
 - radius: radius of the ball -> float or int
 - thicness: set to 0 if you want a solid ball. If set to a non-zero value, then ball will be drawn as a ring and the thickness controls how thick the outline is. -> float or int
 - x & y coordinates: The position of the center of the ball. Note the top left corner is the origin (0,0) and y increases (positive) going down
 - collision sound file: the audio file that gets played when the balls collide the walls of the ring. you can use your own audio files, make sure to convert your audio file to .wav and add it to the audio folder

A possible ball could look like:

```redball_test = Balls("test", (255, 0, 0), 8, 0, width//2, height//2+10)```



## Controls

- press p to pause

That's about it!
