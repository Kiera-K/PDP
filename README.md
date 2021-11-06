## About / Overview : 

The project encompasses a Dungeon game that consists of caves and tunnels which are represented as a 2-dimensional grid. The dungeon can be a non wrapping one or a wrapped one in which case the end caves are connected to the first caves vertically and horizontally. The caves and tunnels can be connected to each other in a maximum of 4 directions and minimum of 1. A player is generated at the start cave of the game which is randomly assigned to the dungeon. The user must move the player from the start to the end cave of the dungeon.

## List of features :
1) Creates a dungeon of caves and tunnels which can be a wrapping or nonwrapping dungeon depending on user input.
2) Randomly assigns a start location where the player will start.
3) Randomly assigns an end location that is 5 hops away from the start.
4) Player can collect treasure from the caves that it visits.
5) Player moves from the start to the end location based on user input.

## How to run       :
Please run the jar file.

## How to use the program : 
A dungeon object is created after taking in user input. A player is generated at a randomly chosen start point. The user is shown the possible moves at
every player position and must choose a move such that the player reaches the end point which is also randomly selected.

# Description of examples :
The output pertains to the user moving the player from the start location to the end location, while collecting treasure along the way. There are 3 files, all of which contain user moves moving the player from start to end. One file is for the wrapping dungeon while the other is for a nonwrapping dungeon. The 3rd file contains the user moves such that the player visits all the caves while moving from start to end in a wrapping dungeon.

## Design/ Model changes :
Changes made :
1) An Edges class was added to incorporate the connections between the caves.
2) The random generator was modified to be seeded.
3) A lot of private methods were added in the dungeon class.

## Assumptions :
1) After the player has pickedup treasure from the cave, the cave is not refilled with any treasure. So if the player goes back to the location, the cave will be empty. 
2) A 5 hop distance is enough to assign the end location randomly. So the end location will always be at the 6th hop from the starting point.

## Limitations:
1) The smallest possible size of the dungeon is 3 X 3 to ensure that the end location at 5 hops away can be reached. A size of 3 x 2 is also possible but the program may not be able to find a path randomly 5 hops away. 


## Citations :
Professor Clark Freifeld
TA - Tanay Joshi
TA - Jaynil Patel

