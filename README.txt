/*
*	Ben McCormack
*	04/02/2026
*/

The A* Pathfinding algorithm is a way for a computer to find the shortest path between two points on a grid or graph.
Typically used for determining the best value path a programme can take to reach a goal where speed and efficiency are important.
A* balances between two factors: the cost to reach a node (g) and an estimate of the cost to reach the goal from that node (h) using the formula f(n) = g(n) + h(n) where f(n) is the total estimated cost of the cheapest solution through node n.
It treats spaces or "steps" as nodes in a matrix assigning values to each node based on the cost to reach it and the estimated cost to reach the goal from there.

This project aims to demonstrate a simple understanding of the algorithm by demostraing it on a 10x10 ASCII grid with randomly placed obstacles.
For example:
			0 0 0 # # 0 # 0 # ?
			0 # 0 # 0 0 # 0 # 0
			0 # 0 0 0 # 0 0 0 0
			# # # # 0 # # # # 0
			# 0 0 0 0 0 0 # 0 0
			0 0 # # # # 0 # # 0
			0 # 0 0 0 0 0 0 # 0
			0 # # # # # # 0 # 0
			0 0 # 0 0 0 0 0 # 0
			! 0 # # 0 # 0 0 0 0

Where '0' represents open spaces, '#' represents obstacles, '!' is the start point, and '??' is the goal point.
When the algorithm runs, it will find the shortest path from '!' to '?', avoiding obstacles and marking the path with '#' characters.
It should output a visual representation of the grid before and after the pathfinding process, along with the steps taken to reach the goal, using '/' to indicate the path found.
For Example:
			0 0 0 # # 0 # 0 # ?
			0 # 0 # 0 0 # 0 # /
			0 # 0 0 0 # 0 0 0 /
			# # # # 0 # # # # /
			# / / / / / / # 0 /
			/ / # # # # / # # /
			/ # 0 0 0 0 / / # /
			/ # # # # # # / # /
			/ 0 # 0 0 0 0 / / /
			! 0 # # 0 # 0 0 # #

This is just an example of how I could go about my project, and I may choose to implement it differently.
There are marks going for demonstating my creaivity and initiative so I may not use this example as something similar to this was used as an example in the explanation.

/*
*	Ben McCormack
*	18/02/2026
*/

Ideas:
1.	Mimic the villager pathfinding in Minecraft
2.	Make a text based wifi bus network that can work between any point. 
3.	Make an elevation based program to find the lowest path. This one seems fun

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Villager pathfinding in Minecrasft assigns blocks a variable based on the type of block and the surrounding blocks. 
Regular blocks being a one, water being a 5, harmful blocks being a 10 or higher depending on the severity of the harm (e.g. cactus is 15 and lava being a 50).
These values also have an affect on their surrounding blocks, combining its own score with a third of the score of it's adjacent blocks rounded down 
	(e.g.  a normal block(1) with water(5) on one side and more normal blocks on the other would have a value of 2)
	(e.g. a normal block(1) with lava(50) on one side and more normal blocks on the other would have a value of 17)
	
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

A text based wifi bus network would be dificult to dress up for presentation but would be a good demonstration of the algorithm.
Object oriented, this one is probably more impressive but labour intensive.
Would be an impressive thing to put in my portfolio but doesn't reflect my interests in the industry as much as the other options.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

An elevation based program to find the lowest path would be a fun project to work on and would be a good demonstration of the algorithm.
If i pixelate a noise map or a height map and assign value of increasing size based on intensity/elevation I could use the A* algorithm to find the lowest path between two points on the grid.
There is merit to this in a practical application as well, as it could be used to find the best path for a hiker or a vehicle to take in a mountainous area, it may even have use in fiction as river
routing or something similar.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The villager pathfinding is the most straight forward to implement as it is a simple grid method dressed up with additional features. I would prefer to work on the elevation idea as it is more 
original and interesting. The trouble is that it would imply an ability to pixelate and assign those values to a grid which is less straight forwward and frankly a bit beyond the current scope of the 
task. 