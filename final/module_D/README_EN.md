# Module D - Creating an interactive module

**Competition time for the task: 4 hours**

![snakegame](/module_D/snake.webp)
In this module, you will create an interactive snake game. The idea is the same as the snake game made by Nokia, but here, you control two snakes simultaneously. The game should look and feel like a real retro game.
The game should be available at the URL: `/games/snakegame`

## Game Start

The game starts with a "Start" button.

## Game functionality

In the game, the player controls two snakes simultaneously. The first snake is controlled with the ADWS keys, and the second with the arrow keys. The snake moves in four directions (up, right, down, and left). Randomly appearing "apples" in the game can be eaten by the player to gain points (one point per apple), and the snake grows in length (one additional point). When the player crosses the edge of the game area, the snake moves to the opposite side of the screen. The game ends when the snake collides with itself or the other snake.

## Game end screen

The game ends with an end screen displaying the score.
Additionally, the question "Do you want to save the score?" is shown to the player. The player can choose "yes" or "no":

- If the player chooses "yes," a name input field and submit button will appear. After entering the name (mandatory), the results (username, score, date, and time) are saved in the database, and a success message is displayed along with a "play again?" button.
- If the player chooses "no, “ the "play again?" button will appear.

## Hall of Fame update

If the player chooses to save the score, the player's name and score are displayed on the game's Hall of Fame list from the database.

**You need to deliver Modules C and D in the end of competition day:**

- A working website that uses a database.
- The final GitHub repository.
- A `README.md` file containing instructions for the intranet and the game.
