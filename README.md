# Machine Learning Project

## Process and Compare Gene Sequences by Using Ant Colony Algorithm

Sequence multiple alignment is a very important operation in bioinformatics, especially in biological sequence analysis. We can use a traditional natural heuristic algorithm, ant colony algorithm, to solve the problem of multiple sequence alignment. The main idea of this algorithm is to use artificial ant colony to select the characters in each sequence one by one. In this process, the ant determines the probability of selecting characters in each sequence according to the information of pheromone, character matching score and position deviation. This strategy is a combination of pheromone updating and adjustment, which can effectively solve the problem of local convergence and strengthen the ability of the algorithm to find the global optimal solution. In this project, we selected some chimpanzee gene sequences as our data set. We will use the above algorithm to deal with and solve the problem of chimpanzee gene sequence alignment.

### Multiple Sequence Alignment
Multiple sequence alignment is a key problem in the fields of bioinformatics and biological sequence analysis. It plays an important role in gene recognition, protein structure prediction, genome information analysis, biological evolutionary tree construction and so on.

Assuming that we know the function of a gene, we can compare the gene with all fragments in the genome database. By observing the comparison results, if a sequence is very similar to the gene, we can infer that their functions are also similar, and they may be homologous sequences. For a series of homologous proteins, studying the relationship hidden in the protein sequence can better understand the evolutionary process of these proteins. Therefore, if we want to find the commonness of multiple sequences, we must compare multiple homologous sequences at the same time.

### Ant Colony Optimization
Ant colony optimization algorithm is a bionic optimization algorithm that simulates the foraging behavior of real ant colonies in nature. It simulates the process of ants looking for food, it can find the shortest path from the origin, through several given demand points, and finally return to the origin. Ant colony optimization also solves the famous traveling salesman problem.

In nature, each ant will leave a substance called pheromone on the route when foraging. Ants transmit information by sensing the concentration of this substance. When choosing the path, ants always tend to move towards the direction of high information cable concentration, and more ants walk on the path with short distance, leaving more pheromones, and the probability of subsequent ants choosing it will be greater; Pheromones on other paths will volatilize over time, which forms a positive feedback mechanism. Finally, the whole ant colony gathers on the shortest path. The brief basic principle of ant colony algorithm is as follows:

- Ants release pheromones on the path.

- When you encounter an intersection that you haven't walked through, choose a road at random. At the same time, pheromones related to path length are released.

- The pheromone concentration is inversely proportional to the path length. Later, when the ants encounter the intersection again, they choose the path with higher pheromone concentration.

- The pheromone concentration on the optimal path is increasing.

- Finally, the ant colony finds the optimal feeding path.

In the first step of each iteration, each ant stochastically constructs a solution, i.e. the order in which the edges in the graph should be followed. In the second step, the paths found by the different ants are compared. The last step consists of updating the pheromone levels on each edge.The brief steps of the Ant colony optimization algorithm are as follows:
- Initialization.
- Select the next node for each ant.
- Update the pheromone matrix.
- Check termination conditions.
- Output optimal value.

