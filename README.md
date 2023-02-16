# Space-Invaders

![Game-Over](https://user-images.githubusercontent.com/91551415/214528728-04894819-319f-4b6f-8f27-36b57426139b.PNG)
## Description
This is the project from the course called "How to Code: Simple Data" by UBCx.

The Space Invaders is a interesting arcade video game using Beginning Student Language (BSL) within DrRacket. 

**Goal:** defeat waves after waves of descending aliens with a missle-shooting tank.

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
		- **on-tick**: An event handler to tell the program to tick in a given rate.
		- **to-draw**: A function to render the image of the game according to its state.
		- **on-key**: An event handler to tell the program to read every keystroke from the user and react accordingly.
		- **stop-when**: Takes a boolean function and a image. Render the image if the boolean function return true

## Code Implementation
The implementation is simple. 
1. Start with a single function big-bang (root).
2. Split the function into several functions (node) with each function doing their own purpose.
3. These functions can be further split into smaller functions, fulfilling smaller tasks.
4. The splitting ends when the "leaf" function require no more splitting.
5. The whole program can be viewed as a giant tree, with the big-bang function at the root.

## How to play the game
1. Download the "space-invaders-starter.rkt" file.
2. Open the file with DrRacket, feel free to browse through the code to see the internal implementation
3. Run the program by clicking the **"Run""** button at the top right. You should see **"All 89 tests passed!"**
4. type **(main (make-game empty empty T0))** in the interacting window (the bottom panel) to start the game.
4. Enjoy it and try not to die!


