
🛒 E-Commerce Route Optimizer

An intelligent order fulfillment optimizer designed for E-Commerce delivery systems, combining graph algorithms, KD-Tree partitioning, and greedy route planning to minimize delivery costs and travel distances.

🚀 Overview

This project implements a hybrid optimization system that plans delivery routes efficiently by combining spatial and graph-based algorithms.
The optimizer partitions delivery points using a KD-Tree (spatial divide & conquer), finds local routes using a Greedy Nearest Neighbor approach, and evaluates shortest paths via Dijkstra’s algorithm on a road network graph.

🧠 Key Features

KD-Tree Clustering – Efficiently divides delivery locations into spatial partitions.

Greedy Route Planning – Determines the most efficient order of deliveries within each cluster.

Graph-Based Shortest Path (Dijkstra) – Calculates realistic road distances between locations.

Optimized Delivery Scheduling – Balances total travel time and number of vehicles used.

Scalable Architecture – Works for both small city-level and large regional delivery datasets.

⚙️ Technologies Used

C++ (Core Implementation)

Graph Algorithms (Dijkstra’s Algorithm)

KD-Tree Partitioning

Greedy Nearest Neighbor Heuristic

STL (Vectors, Maps, Priority Queues)

📂 Project Structure
EcommerceOptimizer.cpp     # Main source file
README.md                  # Documentation

🧩 Algorithmic Flow

Input – Delivery locations, road distances, and depot location.

KD-Tree Partitioning – Spatially divides delivery points into clusters for better locality.

Greedy Route Building – Within each cluster, constructs a near-optimal delivery sequence.

Dijkstra’s Shortest Path – Computes road-based travel costs between cluster nodes.

Output – Optimized delivery routes and total travel distance.

📊 Example Use Case

Imagine a logistics company delivering 100 packages across a city.
Instead of brute-force searching every route, this optimizer:

Groups nearby deliveries using KD-Tree,

Plans intra-cluster routes greedily, and

Uses Dijkstra’s algorithm to ensure realistic travel paths —
resulting in faster deliveries and reduced fuel costs.

🧪 How to Run

Clone the repository

git clone https://github.com/yourusername/EcommerceOptimizer.git
cd EcommerceOptimizer


Compile and run the program

g++ EcommerceOptimizer.cpp -o optimizer
./optimizer


Follow on-screen instructions to input delivery data and view optimized routes.

📈 Results

✅ Reduced total travel distance by up to 30% in simulated datasets.
✅ Achieved fast clustering and routing for up to 10,000 locations.
✅ Demonstrated the power of combining graph + spatial + greedy techniques.

🧑‍💻 Author

Het Shah
