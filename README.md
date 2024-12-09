Friends Game - Snake Game Implementation
Overview
This Python script creates a simple snake game using the Turtle graphics library. The player controls a snake that moves around the screen, eating food to grow longer while avoiding collisions with the walls and itself. The game keeps track of the player's score and high score.

Key Components
Libraries Used
turtle: A standard Python library for creating graphics and simple games.
time: Used for adding delays in the game loop.
random: Used to generate random positions for the food and random colors/shapes.
Game Setup
Screen Setup:

The game window is created with a title "Friends Game" and a green background.
The window size is set to 600x600 pixels, and the screen updates are turned off for smoother animations.
Snake Initialization:

The snake's head is represented as a black square, initially positioned at the center of the screen (0, 0).
The snake's movement direction is initialized to "Stop".
Food Initialization:

The food is represented by a randomly chosen shape and color, initially placed at (0, 100).
Score Display:

A turtle object is used to display the current score and high score at the top of the screen.
Movement Functions
Functions are defined to change the direction of the snake:
group(): Moves the snake up.
godown(): Moves the snake down.
goleft(): Moves the snake left.
goright(): Moves the snake right.
The move() function updates the position of the snake based on its current direction.
Game Loop
The main game loop runs indefinitely, performing the following tasks:

Screen Update: The screen is updated to reflect changes.
Collision Detection:
If the snake collides with the wall, it resets to the center, and the score is reset.
If the snake eats the food, a new food item is generated at a random position, and a new segment is added to the snake's body. The score increases, and the high score is updated if necessary.
Segment Movement: The segments of the snake follow the head, creating the effect of movement.
Self-Collision Detection: If the snake collides with itself, it resets similarly to wall collisions.
Delay: A delay is added to control the speed of the game.
Controls
The player can control the snake using the following keys:
W: Move up
S: Move down
A: Move left
D: Move right
Conclusion
This simple snake game provides a fun way to practice programming with Python and the Turtle graphics library. Players can enjoy the challenge of growing their snake while avoiding collisions, and the game keeps track of their scores for added competition.
