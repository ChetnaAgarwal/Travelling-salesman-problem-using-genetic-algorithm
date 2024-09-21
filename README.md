# Travelling-salesman-problem-using-genetic-algorithm

Results available at : https://drive.google.com/drive/folders/1ouA5AsMy_r5lZv1Ff5z3GRw3yAaaXKSR?usp=sharing

## Objective:
The goal is to find the shortest route traversing a set of planets (similar to the Traveling Salesman Problem) using a genetic algorithm.

## Key Components:

1. Environment Class:

Represents the setting with planets and their distances.
Contains methods to reset the environment and step through actions, returning the distance traveled.

2. Route Class:

Encapsulates the DNA (route) consisting of a sequence of planets.
Initializes with random DNA and includes methods for:
- Mixing (Crossover): Combines two parent routes to create a new route, enhancing genetic diversity.
- Mutation: Introduces random changes to the DNA to prevent premature convergence.

3. Population Initialization:

Creates an initial population of random routes (bots) based on the number of planets.
Each route's fitness (total distance) is calculated using the environment’s step method.

4. Main Loop:

Iterates through generations, performing the following:
- Evaluation: Calculates the distance for each route and sorts the population based on fitness.
- Selection: Preserves a certain number of the best routes for the next generation.
- Crossover and Mutation: Fills the rest of the population either with random routes or offspring from selected parents.
- Display: Shows the best route found every 100 generations and tracks the shortest distance.

5. Termination Condition:

The main loop runs indefinitely, but it can be enhanced with a condition to stop after a certain number of generations or if improvement stagnates.


## Important Highlights:
- Genetic Algorithm Principles: Utilizes selection, crossover, and mutation to evolve the population over generations, aiming for optimal solutions.
- Dynamic Population: Balances between preserving successful routes and introducing new variations, maintaining genetic diversity.
- Real-Time Feedback: Provides visual feedback on the best route, enhancing understanding of the algorithm's performance over time.


## Conclusion:
This project effectively demonstrates the application of genetic algorithms in solving optimization problems, specifically finding efficient routes through a series of points. It showcases fundamental AI principles and offers a framework that can be adapted for other similar problems.
