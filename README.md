# Graph-Coloring-Using-Genetics-Algorithm

# Objectives
The main aim of the program is to develop different approaches for graph coloring, while focusing on genetic algorithms and backtracking techniques. Furthermore, the objective is to assign colors to the nodes of a graph so that no two neighboring vertices share the same color. This project aims to provide a way for efficiently coloring graphs with the fewest amount of colors.
# Importance
Graph coloring has numerous applications in fields such as timetabling problems, scheduling problems, job allocation problems, team building problems, and more. An efficient graph coloring algorithm can lead to significant performance improvements in these areas.

# Main Functionalities
1.	Graph Input Methods: 
•	Adjacency List 
•	Adjacency Matrix
•	Adjacency Dictionary 
•	Random Generated Graph
2.	Graph Coloring Algorithms:
•	Genetic Algorithm
•	Backtracking Algorithm

# Input and Output Format
Input Format:
1.	The program asks the user to enter the number of graph nodes.
2.	The program asks the user to enter the number of the population size.
3.	The program asks the user to choose what type of input graph wants from the following choices:
	•	List (The program will ask the user to enter an adjacency     list for each node (separate neighbors by space))
	•	Matrix (The program will ask the user to enter an adjacency matrix)
	•	Dictionary (The program will ask the user to enter an adjacency dictionary (node: [list of neighbors]))
	•	Random Graph (Will generate random graph)

![alt text](https://github.com/Doaa-Mahdy/Graph-Coloring-Using-Genetics-Algorithm/blob/Images/in.png?raw=true)


# Output Format:
•	First determine the maximum number of connections to the nodes 
•	It prints the graph using the maximum number as the number of node colors  
•	Then decrease the colors one by one until a minimum number of colors is used
•	The final outputs are the graph with the minimum color used , the greedy solution, backtracking proof, and how many colors are used.
![alt text](https://github.com/Doaa-Mahdy/Graph-Coloring-Using-Genetics-Algorithm/blob/Images/out.png?raw=true)

Details of the algorithm(s)/approach(es) used and the results of the experiments.
# 	Genetic Algorithm
1.	Generate an initial population of chromosomes, where each chromosome represents a possible color of the graph.
2.	Calculate the fitness function of each chromosome based on the number of conflicts (adjacent vertices having the same color).
3.	Select the fittest individuals from the population for reproduction. Two selection methods were implemented:
i.	Truncation Selection
ii.	Tournament Selection
4.	Combine pairs of parents to produce offspring using methods like One-Point Crossover and Two-Point Crossover
5.	Introduce random changes to offspring to maintain genetic difference.
6.	Repeat the selection, crossover, and mutation steps until a correct color is found or a maximum number of generations is reached.
# Backtracking Algorithm
1.	Color each node using a recursive function that assigns colors and backtracks if a conflict is found.
2.	Ensure that no two adjacent vertices have the same color before assigning a color.
3.	Continue the process until all nodes are colored without conflicts.
# Experiment Result 
•	Various sizes of graphs (small to large) were tested.
•	Different population sizes were used for the genetic algorithm.
•	The algorithm was run for varying numbers of generations.
# Findings
•	The genetic algorithm was able to find valid colorings for most graphs within a reasonable number of generations.
•	The backtracking algorithm guaranteed a solution but was slower for larger graphs due to its recursive nature.
•	The number of colors required varied depending on the graph's structure and size. In some cases, the genetic algorithm found colorings with fewer colors compared to the backtracking method.
Images output. 

