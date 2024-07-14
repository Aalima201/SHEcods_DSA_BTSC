QUESTION 1 EXPLANATION :
Explanation:


Data Structures:

graph is an unordered_map where each key is a city (string) and the value is a vector of pairs, representing neighboring cities and the travel times to them.


Adding Edges:

The addEdge function adds an edge between two cities with the given travel time.


Updating Travel Times:

The updateTime function updates the travel time for a specific edge in the graph.


Dijkstra's Algorithm:

The dijkstra function finds the shortest path from the start city to the end city with an optional parameter k for the number of stops.
A priority queue (min-heap) is used to always expand the least costly node next.
The distances map keeps track of the shortest known distance to each city.
The function returns the shortest distance to the end city that meets the criteria, or infinity if no such path exists.


Finding Best Routes:

The findBestRoute function iterates over a list of k values and finds the shortest path for each using the dijkstra function.


Driver Code:

Initializes the RouteBuddy instance with the sample data.
Applies traffic updates.
Finds the best routes for different k values before and after traffic updates.


Output:

The results are printed, showing the best routes before the traffic updates.

