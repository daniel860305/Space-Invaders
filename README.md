# Space-Invaders
This is the project from the course called "How to Code: Simple Data" by UBCx.

The Space Invaders is a interesting arcade video game using Beginning Student Language (BSL) within DrRacket. 

Your goal is to defeat wave after wave of descending aliens with a horizontally moving tank.

## Domain Analysis
During the domain analysis phase, there are mainly four parts to consider:
- **Scenario**:
	- Visualize what the game should look like
	- Consider some user cases using illustrations
- **Constant**:
	- This is the point to identify components that should be constant
	- constant components include images of tank, aliens, missiles, etc (see the picture of "Domain Analysis.jpg").
- **Changing**:
	- Need to identify all changing components in the game.
	- These components change dynamically in different user scenarios
	- The crucial part of the game design
- **Big-bang options**:
	- BSL with 2htdp/universe module provides useful functionality for creating interactive, graphical programs.
	- I use big-bang functions with 4 clauses to create an interactive game:
		- **on-tick**: tell the program to tick in a given rate.
		- **to-draw**: tell the program to render the image of the game.
		- **on-key**: tell the program to read every keystroke from the user and react accordingly.
		- **stop-when**: indicate the program when to stop the game and show the game-over image.

## Implementation
The implementation is simple. 
1. I start with a single function big-bang (root).
2. I split this function into several functions (node) with each function doing their own purpose.
3. These functions can be further split into smaller functions, fulfilling smaller tasks.
4. The splitting ends when the "leaf" function require no more splitting.
5. The whole program can be viewed as a giant tree, with the big-bang function at the root.

## How to play the game
1. Download the "space-invaders-starter.rkt" file.
2. Open the file with DrRacket, feel free to browse through the code to see the internal implementation
3. Run the program. After you see **"All 90 tests passed!"**, type (main (make-game empty empty T0)) to start the game.
4. Enjoy it and try not to die!


