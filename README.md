# Genetic Algorithm Car Racing Game
## Introduction
This repository contains a project that applies a genetic algorithm to a car racing game, enabling automated navigation through a set of checkpoints on a predefined track. The project is designed as part of a course at the National University of Computer and Emerging Sciences. It focuses solely on the implementation of the genetic algorithm, as the game environment is pre-coded.

## Game Mechanics
Each car in the game is equipped with five sensors (left, top left, top, top right, right) that detect proximity to the track walls. The car's movements are dictated by these sensors and predefined movement values (1: forward, 2: backward, 3: left, 4: right). A car's behavior in the game is determined by a chromosome—a dictionary mapping sensor inputs to movement outputs.

## Genetic Algorithm Overview
The genetic algorithm optimizes the car's ability to navigate the track by evolving the chromosomes over successive generations. Each generation consists of 30 cars attempting to complete the track:

 - **Fitness Evaluation:** Cars are scored based on the number of checkpoints crossed.
 - **Selection:** Cars with higher scores have a greater chance of passing their genes to the next generation.
 - **Crossover and Mutation:** Chromosomes of selected cars are crossed over and mutated to produce offspring for the new generation.
 - **Termination:** The algorithm terminates if a car successfully navigates all checkpoints without collision or upon reaching a time limit, which adjusts based on the performance of the best car in the previous generation.

## Important Points
 - All cars are instances of the AgentCar class.
 - Mutation should only alter the values of the chromosome within the range [1, 4].
 - Extensive debugging via print statements is recommended due to minimal error handling in the game code.
   
## Running the Game
To run the game and observe the performance of the genetic algorithm, follow these steps:
 - Clone the repository to your local machine.
 - Execute the game script on your Jupyter Notebook or VS Code with Python extension to start the simulation.
 - Observe the algorithm's performance across generations.

Below is a screenshot demonstrating the game started in action. 
  
![startgame](https://github.com/Maryam189/Genetic-Algorithm-Car-Racing-Game/assets/76420523/c9ac1109-b23c-4a73-9610-8dceee9e5bf7)

Below is a screenshot of the game in which car reaches its final Goal State.

![wingame](https://github.com/Maryam189/Genetic-Algorithm-Car-Racing-Game/assets/76420523/4f14781d-bc3d-4100-a7fe-f4bb5a8a73f7)

The visualization helps in understanding how the cars navigate the track using the genetic algorithm.


## Conclusions and Observations
The project showcases the effectiveness of genetic algorithms in solving complex pathfinding problems in dynamic environments. Observations on the algorithm's performance and potential areas for improvement are discussed in detailed project documentation.

## Contributing
**Contributions are Welcome!** Please send me a pull request or open an issue to discuss your ideas. If there's anything else you'd like to know about it, let me know. Feel free to reach me out at Maryamkhalid590@gmail.com
