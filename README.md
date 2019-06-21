# Tabu Heuristics for Capacitated Vehicle Routing

- IT252 Desgin And Analysis of Algorithms (DAA) course project: Vehicle Routing Problem or simply VRP is a well known combinatorial optimization problem and a generalization of the travelling salesman problem. A definition of the problem is this: We have a number of customers that have a demand for a delivery. Which are the optimal (minimal) routes for a fleet of vehicles starting from a single point (depot) to deliver the requested goods in all customers. Finding optimal solution is a NP-hard problem so heurestic strategies are proposed for approximation of the optimal solution.
- For more about the problem see: https://en.wikipedia.org/wiki/Vehicle_routing_problem

# Usage

- The implementation is in Java. The code itself is in a single class named "VRP.java". A greedy solution was calculated at first and then three heuristic strategies where tested against it. 
- Intra route where a customer can be reassigned in a different position in the same route, inter route where a customer can be reassigned in another position in the all vehicle routes and Tabu search where we keep selecting the best neighboor solution even if it it is worst than the current solution for a number of iterations.

# Output

- This code prints the solution from each strategy in console and creates 4 png images for all solutions (Greedy, IntraRoute, InterRoute, Tabu) and 3 files for the evolution in solution costs for the heuristics algorithms. 

# Analysis

- Tabu search has the best perfomance; for an instance of the problem where we had 30 random placed customers and 10 vehicles: Greedy solution was 793 distance units (du), Intra Route Heuristic Algorithm gave 761 du , Inter Route 644 du amd finally Tabu Search gave 637 du after 200 iterations. 

- Tabu search has the flexibility to overcome local minimum so this is why we expect to be the beter strategy. In the next two images we can see the initial greedy solution graphicxally represented and the final solution the came from Tabu search. 


# Presentation
The Presentation PDF is available here : https://github.com/Rakeshpavan333/daa_pro/blob/master/daa_pro.pdf

# Team

- Rakesh Pavan (17IT154)
- Dhruvik Navadiya (17IT225)
- Neeraj Deshpande (17IT226)
- Yogesh Choubey (17IT252)
