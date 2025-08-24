# Vehicle_Routing_Optimization
This project implements a Genetic Algorithm (GA) to solve the Vehicle Routing Problem (VRP) using the DEAP framework in Python.

The VRP is a classic combinatorial optimisation problem where a fleet of vehicles must serve a set of locations starting and ending at a depot, minimizing the total travel distance while balancing the workload among vehicles.

Features:

Implemented with Genetic Algorithms (GA) using the DEAP framework.

Custom fitness function considering:

1. Total distance travelled by all vehicles.

2. Standard deviation of route lengths (to balance vehicle workloads).

## How It Works:

Representation:

Each individual represents a permutation of customer visits, assigned cyclically to vehicles.

Fitness Function:

Computes the total distance traveled.

Measures the balance of workload using standard deviation of route distances.

def evalVRP(individual):
    # Returns (total_distance, distance_std_dev)

Genetic Operators:
Selection: Tournament / Roulette wheel.

Crossover: Ordered crossover (OX).

Mutation: Swap mutation.

Optimization Goal:

Minimize total travel distance while maintaining balanced vehicle routes.

** Future Improvements

Add capacity constraints for vehicles.

Extend to VRPTW (Vehicle Routing Problem with Time Windows).

Interactive route visualization.

Compare GA with other metaheuristics (e.g., PSO, ACO, Tabu Search).
