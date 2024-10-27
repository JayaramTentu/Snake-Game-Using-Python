# Snake-Game-Using-Python

This design creates an interactive, continuous play Snake game with simple yet effective animations, screen wrapping, and a responsive control system, making for a fun user experience.

       Python code uses the turtle graphics library to create a classic "Snake" game with a few custom features. Here’s a summary of how the game is designed and functions:

# Running :

 https://github.com/user-attachments/assets/575e7b96-a484-48aa-8354-23c95bf51dcd

 
# Game Area Setup:
    
    The game window is a 500x500-pixel square with a black background.
    The snake moves within the boundaries, but the design allows for screen wrapping—when the snake exits one side of the screen, it reappears on the opposite side, 
    creating a continuous movement environment.
    
# Snake Initialization:

    The snake starts with a series of yellow square segments arranged vertically, initially moving "up."
    The snake variable is a list of coordinates representing each segment, with the snake’s head being the last element.

# Snake Movement:

    Movement is determined by the current direction, stored in snake_direction, and updated based on arrow key input.
    Each time the snake moves, it adds a new head position in the current direction, and if no food is eaten, the tail segment is removed, maintaining its length.
    Collision detection checks if the snake collides with itself (in which case it resets), and screen wrapping logic ensures it reappears on the opposite side when it goes out of bounds.

# Food Placement and Collision:

    Food is represented by a red circle and placed randomly on the screen.
    When the snake head collides with the food (based on proximity), the food relocates, and the snake grows by one segment.
    The function food_collision handles detecting when the snake eats the food.
