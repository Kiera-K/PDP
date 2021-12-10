## PROJECT 5

## 1. Overview:

This project provides a graphical user interface(GUI) for playing the dungeon game. The GUI initially begins with a popup
asking the user to input the dungeon specifications. The bespoke dungeon is then rendered onto the screen. The user can 
use either the arrow keys or mouse clicks to navigate the player about the dungeon, while picking up arrows and/or
treasure as and when he finds and for shooting the arrows in the direction and distance desired. The GUI also has an option 
to check the player description at each stage of the game. The entire dungeon is initially obscured from the user and he must 
explore the different paths of the dungeon to find the end cave and complete the game. The dungeon has elements that work 
against the player, namely otyughs, pits and a thief. The thief is sly and randomly jumps locations.
The user must nagivate vigilantly so as to avoid being killed by otyughs and avoid falling into pits.  
The user must maneuver the player to avoid all these obstacles and reach the end cave without getting eaten by the end cave otyugh
to win the game.

## 2. List of features: (including some extra credit features)

1) The dungeon game begins when the controller calls the playGame() method. It initializes the Graphical User Interface (GUI), that begins 
with a popup asking the user to enter the desired configuration of the dungeon.

2) Once the GUI is rendered, the user can see the cave of the dungeon that the player is in and the possible directions to move, 
 along with other items that are present in that cave that can include arrows, treasures, otyughs, pits and a thief.
3) The user can move the player in the desired direction using the arrow keys on the keyboard or using mouse clicks.
4) The user can pick up arrows using the "A" key, pick up treasure using the "T" key and shoot an arrow using the "S" key on the keyboard.
5) The GUI also warns the player whether an otyugh is near by and how near by showing a green ball of stench. If the greenness is darker, 
the otyugh is closer.
7) The GUI provides functionality for checking the player's description at each stage of the game.
8) It also has options for viewing the configuration of the current dungeon.
9) The user can also restart the game either with the old configuration of the dungeon or enter in, new specifications of the dungeon.

## 3. How to run:

The game can be run either in the GUI mode or the text based mode.
The game begins with an option that is given to the user. If the args are passed to the program, the game begins in text based mode.
Otherwise it starts in the GUI mode.

Please run the jar file to play the game.

To play the GUI mode, you can put in the values in the initial prefilled popup that asks for the configuration of the desired dungeon.

In case of text based mode, the order of the arguments are as follows : 
1) m : number of rows of the dungeon
2) n : number of columns of the dungeon
3) interconnectivity : interconnectivity of the dungeon
4) treasurePercentage : Percentage of caves that should have treasure.
5) monsterCount : The number of otyughs that should be present in the dungeon.
6) isWrapped : Whether the dungeon should be wrapping or not.

Example values : 4 6 6 20 3 y
     
## 4. How to use the program:

In the GUI mode, after initializing the dungeon you can use the:

A key : To pick up arrows.
T key : Tp pick up treasure.
S Key : To shoot an arrow. This is followed by popups for accepting the distance and direction in which to shoot the arrow.
Arrow keys to move the player up, down, left and right.
or 
Mouse clicks to move the player in the desired direction.
The user is informed of any otyughs nearby by displaying a green ball of stench. If the greenness is darker, 
the otyugh is closer.

Run the jar file with either arguments as mentioned above in the order => (m n interconnectivity treasurePercentage monsterCount, isWrapped) 
or 
without arguments to enter the GUI mode.

## 5. Description of examples:

Screenshots attached.

## 6. Design Changes: (Extra credit features)

1. Initially I thought the view would have only a view class and a panel. But then I had to create a number of other classes 
to override ActionListeners and MouseAdapters and also create customActionListeners.
2. I added the extra credit features for the final design which I had not thought about in the intial design. So my final 
design also contains a thief interface
and incorporates pits that the player could fall into.

## 7. Assumptions:

1. The player has 4 lives. Each time the player falls into a pit, he must use a life to jump out of the pit. Once all lives are used,
and the player falls into another pit, the player's health is set to false and the player dies.
2. The thief moves around the dungeon randomly each time the player moves. When the player and the thief come into the same cave, the thief
steals all the treasure that the player has collected. But the player's life remains unharmed.
4. The amount of treasure collected does not get converted into lives for the player.
5. There can be multiple arrows in a cave.
6. If arrows are found in a cave, and the user decides to pick, the player must pick all arrows and not just a specified number.
7. Similarly, if treasure is found, and the user decides to pick, the player must pick all the treasure instead of just a specific one like only ruby.
8. When a player escapes an injured monster by a probability of 50%, the player and the injured monster coexist in that cave.

## 8. Limitations:

1) The player has only 4 lives. (player health and player lives are 2 separate attributes)
2) When the thief steals treasure from the player, the player cannot fight back for it.
3) The player will never find a thief in a tunnel.
4) The player health does not have levels and can take only 2 values : Alive or dead. (True or false)
5) There can be only 1 monster per cave.
6) There can be only 1 player per dungeon.

## 9. Citations:

1) Professor Clark Freifeld
2) Sean Maloney

