Project-Title:
GUI Based Multiplayer Battleship Online Game

Project-Implementation:
It’s a multiplayer game, two players will be playing a match who hit on “Start Game” simultaneously or at least within 10sec. If a player doesn’t find any opponent even after waiting for 10sec, then computer automatically starts playing with him. The application have a graphical user interface that displays the current status of game, with a 2D representation of the player's grid with ship positions and hit squares, and another grid representing which squares the player have shot at.

Project-Interface:
• Two windows, one for player1 and other for player2
• Initially both the windows contain option to either start the game or to quit the game
• In the game mode, each window contains two grids. One grid keeps the track of his opponent ships which he destroyed or sunk and the other contains his arrangement of ships

Project-Description:
Battleship is a game where the player has to find and sink all ships of the opponent. The game is played with two players sitting opposite to each other so they will not see each-others grids.
Each player will have a battleship game unit with 3 ships and an additional grid where they can keep track of their guesses (with red and white colours on the cells of the grid). The ships are the Destroyer (of length 1 unit), the Submarine (of length 2 units) and the Battleship (of length 3 units). Players will position their five ships on their respective grids (either vertically or horizontally).
The objective of the game is to sink all your opponent’s ships. A ship will occupy spaces on the grid which will be a 5 X 5 matrix with columns labelled from A to E and rows from 1 to 5. Players take turns marking out (on the additional grid) some coordinates looking to hit a ship.
A ship is sunk when all holes on the ship have been hit (guessed correctly). The other player will locate the coordinate and respond hit or miss (here the corresponding cell colour on the additional grid of first player will be changed to red if it’s a hit or to white if it’s a miss).If it’s a hit, then the colour of the corresponding cell of the ship will be changed to red.
The player who destroys all his opponent’s ships is the winner.

User requirements:
Pygame

Game rules:
• A ship coordinates should not be out of the range of the grid coordinates
• A ship cannot overlap other ship in the same space.
• A ship cannot be placed diagonally.
• Once the game begins all the ships should stay where they are kept initially and cannot be changed

External Packages Used:
This requires a package named “Pygame” which sets up the outer look as well as the logic of the game. To make it online, i.e. to set up a server and a few clients, we include a few additional packages named “Socket”, “Thread” and “Random module”.
We need to use another package named “Pickle” which is used share data among server and clients in form of objects rather than as a string.

Commands to run:

python main_server.py nnnn

python main_client.py nnnn

in different terminals.
