# Tic Tac Toe Game

This repository contains a Java implementation of the classic Tic Tac Toe game. The game can be played between a human player and an AI player. The AI makes random moves, and the game checks for win conditions (row, column, diagonal) or a draw.

## Technologies and Tools Used

- **Java**: The programming language used to implement the game.
- **Java Development Kit (JDK)**: To compile and run Java programs.
- **Integrated Development Environment (IDE)**: Such as IntelliJ IDEA, Eclipse, or NetBeans for writing and debugging code.
- **Command Line Interface (CLI)**: To compile and run the Java files.

## Code Structure

- **TicTacToe.java**: Contains the main logic for the Tic Tac Toe game, including the board initialization, display, and win-checking methods.
- **Player.java**: Abstract class that defines common properties and methods for both human and AI players.
- **HumanPlayer.java**: Extends `Player` and implements the `makeMove` method for human input.
- **AIPlayer.java**: Extends `Player` and implements the `makeMove` method using random moves for the AI.
- **LaunchGame.java**: Contains the main method to run the game, initializes players, and alternates turns until there's a win or a draw.

## Game Logic

### Board Initialization
The board is a 3x3 grid, initialized with empty spaces. The board is displayed with row and column separators for better visual representation.

### Player Moves
- **HumanPlayer**: Prompts the user to enter the row and column for their move, ensuring the move is valid.
- **AIPlayer**: Generates random row and column values for its move, ensuring the move is valid.

### Win Conditions
The game checks for the following win conditions:
1. **Column Win**: Three marks in any column.
2. **Row Win**: Three marks in any row.
3. **Diagonal Win**: Three marks in either diagonal.

### Game Draw
If all positions on the board are filled without any player meeting the win conditions, the game declares a draw.

## Running the Game

To compile and run the game, follow these steps:

1. **Compile the Java files**:
    ```sh
    javac TicTacToe.java Player.java HumanPlayer.java AIPlayer.java LaunchGame.java
    ```

2. **Run the game**:
    ```sh
    java LaunchGame
    ```

## Example Gameplay

```sh
Bob turn
Enter the row and col
1 1
-------------
|   |   |   | 
-------------
|   | X |   | 
-------------
|   |   |   | 
-------------
TAI turn
-------------
|   |   |   | 
-------------
|   | X |   | 
-------------
|   | O |   | 
-------------
Bob turn
Enter the row and col
0 2
-------------
|   |   | X | 
-------------
|   | X |   | 
-------------
|   | O |   | 
-------------
TAI turn
-------------
|   | O | X | 
-------------
|   | X |   | 
-------------
|   | O |   | 
-------------
Bob turn
Enter the row and col
2 0
-------------
|   | O | X | 
-------------
|   | X |   | 
-------------
| X | O |   | 
-------------
Game Draw
```

**Author:** Ravishankar Kumar  
**Email:** [ravishankarmahto887752@gmail.com](mailto:ravishankarmahto887752@gmail.com)  
**Stream:** Software Developer

