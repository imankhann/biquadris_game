# Biquadris

This repository is for the Biquadris game, which served as the final assignment for the CS 246 course at the University of Waterloo.

This project was completed by Iman Khan, Ananya Ohrie, and Larry Chen.

Each Biquadris game features two game boards, each with 11 columns and 15 rows. The objective is to strategically place these blocks onto their respective boards without leaving any gaps.

Unlike Tetris, Biquadris is not played in real-time. Players have unlimited time to make decisions about where to position a block. The game proceeds in turns, with each player taking one turn at a time. A player's turn concludes when they successfully place a block on their board, unless this action triggers a special event. Importantly, the block that the opponent must play next is already at the top of their board during the current player's turn. If this incoming block cannot fit on the opponent's board, the opponent loses the game.

# Special Actions

When a player successfully clears two or more rows with a single block placement, it triggers a special action that has a detrimental impact on the opponent's gameplay. The game will prompt the player to select their desired action from the following options:

Blind: This action obscures the player's board, covering columns 3 to 9 and rows 3 to 12 with question marks (?). The obscured display remains until the player drops a block, at which point it reverts to normal.

Heavy: With this action, whenever a player moves a block left or right, the block automatically drops by two rows after the horizontal movement. If it's not possible for the block to descend two rows, it is considered as dropped, and the player's turn ends.

Force: Choosing this action allows the player to change the opponent's current block to one of their own choosing. However, if the selected block cannot be placed in its initial position on the opponent's board, the opponent loses the game. For example, "force Z" would replace the opponent's block with a Z-shaped block.

# Score

Scoring in the game operates in the following manner: Whenever a line or multiple lines are successfully cleared, you earn points equivalent to the square of the sum of your current level and the number of lines cleared. 

Furthermore, when an entire block vanishes from the screen, meaning that all of its cells have disappeared, you earn points equivalent to the square of your level at the time the block was generated, increased by on

# Arrow Keys

We also implemented a way for the user to use arrow keys.
With our implementation, each command has a letter or arrow key associated with it. If players press & followed by enter/return during their turn, they can take advantage of this block control method until their turn is done or they want to turn it off, which can be done by pressing the letter & again. The commands and their associated letter or arrow keys are shown below:

Arrow Keys			      
levelup = up arrow key
down = down arrow key
left = left arrow key
right = right arrow key
clockwise = x key
counterclockwise = y key
drop = d key
leveldown = a key
random = r key

Letter Keys
I block = i
J block = j
L block = l
O block = o
S block = s
Z block = z
T block = t
restart = e
Default theme = 0 (zero)
Barbie theme = b
Oppenheimer theme = p

# Themes

Another feature we implemented was allowing players to choose their color theme during any part of the game, with the choices being Default, Barbie, and Oppenheimer. At the start of the game, the theme is set to default. If players are in & mode (using letter and arrow keys to navigate), they can change the theme by typing 0 for Default, b for Barbie, and p for Oppenheimer. If the players are in regular game mode, they would enter default for Default, barbie for Barbie, and opp for Oppenheimer


