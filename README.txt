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

