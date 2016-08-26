#Racing Game 

An object-oriented plan for an in-browser car racing game

### User Stories & Game Mechanics
1. Players can see two cars on the racetrack.
2. Each player can make a car move forward with a keypress.
3. The first player to make their car reach the finish line wins!

### Data Structures
1. **Car**
  	* `carImage` (string)
  	* `row` (number)
  	* `positionX` (number)
  	* `positionY` (number)

2. **Track**
	* `image` (string)
	* `finishLine` (number)
3. **Game** 
	* `win()` (function)


### Development Stories

1. Players can see two cars on the racetrack.
  	* Ensure that cars start at same X-coordinate, but different Y-coordinate 	(depending on Car.row value instantiated) 

2. Each player can make a car move forward with a keypress.
  	* Player1 car moves forward with "d" key, while player2 car moves forward 	with "right arrow" key
  	* Attach event listeners for keypresses, with a callback that will update 	the corresponding car image X-coordinate by 10 pixels(?) until a player  	reaches the finish line

3. The first player to make their car reach the finish line wins!
	* Call win function on Game instance when a Car positionY equals the Track 	finishLine


###Potential Challenges / Development Questions
1. How to get each Car image to move? Can the Game render the Track on a loop?
2. Can we make the cars move more continuously than discretely?
3. Can we refresh the images without reloading the page? Will this move slowly?