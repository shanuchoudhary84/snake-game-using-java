# Snake-Game-Java-DSA-
SNAKE GAME USING JAVA (DATA STRUCTURES AND ALGORITHMS)
The code implements a simple Snake game using Java Swing. It sets up a game board where a snake moves around, eats food, and grows. The player controls the snake's direction using arrow keys. The game ends when the snake collides with the walls or itself. The code structure separates game logic, user input handling, rendering, and collision detection for clarity and maintainability.

Sure! Here's a concise summary of the Snake game code in Java:

### Overview:
The code implements a simple version of the classic Snake game using Java Swing for the graphical user interface. The player controls a snake that moves around the game board, eats food, grows longer, and must avoid collisions with the walls and itself.

### Key Components:
1. **Imports:**
   - Import necessary packages for GUI components, event handling, and utility classes.

2. **SnakeGame Class:**
   - Extends `JPanel` to create the game board.
   - Implements `KeyListener` to handle keyboard input.
   - Implements `ActionListener` to handle game updates via a timer.

3. **Constants:**
   - Define the game board size, tile size, and update delay.

4. **Instance Variables:**
   - `snake`: An `ArrayList` holding the coordinates of the snake segments.
   - `food`: A `Point` object representing the position of the food.
   - `direction`: An integer representing the current direction of the snake.
   - `timer`: A `Timer` object to control the game loop.

5. **Constructor:**
   - Initializes the game board, sets up initial snake position, generates the first food item, and starts the game timer.

6. **paintComponent Method:**
   - Overrides the `paintComponent` method to draw the snake and food on the game board using `Graphics`.

7. **KeyListener Methods:**
   - `keyPressed`: Changes the direction of the snake based on arrow key input.
   - `keyReleased` and `keyTyped`: Required for `KeyListener` interface but not used.

8. **ActionListener Method:**
   - `actionPerformed`: Called by the timer to update the game state, move the snake, check for collisions, and repaint the game board.

9. **Game Logic Methods:**
   - `move`: Updates the snake's position and handles food consumption.
   - `generateFood`: Generates a new food item at a random position.
   - `checkCollision`: Checks for collisions with the walls or the snake itself.
   - `gameOver`: Stops the timer and displays a game over message when a collision is detected.

10. **Main Method:**
    - Creates and sets up a `JFrame` to host the game panel, configures window properties, and makes the game window visible.

### Summary:
This code provides a basic implementation of the Snake game with functionalities for moving the snake, growing when eating food, and ending the game upon collisions. The game uses a `JPanel` for the game board, a `Timer` for periodic updates, and `KeyListener` for handling keyboard input.
