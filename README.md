# crossing-game-in-python-with-turtle

This code is for a simple game where the player (represented by a turtle) has to cross a busy road without getting hit by cars. The game board is set up using the Screen module from the turtle library.

The code sets up a Player object (the turtle) and a CarManager object, which creates and moves the cars that the player must avoid. It also sets up a Scoreboard object, which keeps track of the player's score and level.

The screen.listen() method allows the program to listen for key presses. In this case, the Up arrow key is used to move the player upwards.

The while loop runs continuously while the game is on. Within the loop, time.sleep(0.1) is used to create a delay between each frame of the game, and screen.update() is used to update the screen.

The car_manager.create_car() method creates a new car object at random intervals, and the car_manager.move_cars() method moves all the cars across the screen.

The for loop checks for collisions between the player and any cars in the CarManager object. If a collision is detected (i.e., the distance between the player and a car is less than 20), the game is over and the Scoreboard object displays a "game over" message.

If the player successfully reaches the other side of the screen (i.e., crosses the finish line), the player is reset to the starting position, the level is increased, and the Scoreboard object updates the player's score and level.

Finally, the game exits when the player clicks on the screen.
