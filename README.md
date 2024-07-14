QUESTION 1 EXPLANATION :
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



QUESTION 2 EXPLANATION :
Friend Class:

Represents a friend with a name and follower count.


updateFollowers Function:

Updates the follower count of a given friend.


getMostInfluentialFriends Function:

Sorts the friends in descending order based on their follower count.
Returns the top 4 friends as the most influential.


Main Function:

Initializes Rajat's friends with their initial follower counts.
Updates the follower counts based on the provided changes.
Adds new friends.
Determines and prints the most influential friends.


QUESTION 3 EXPLANATION :
FileSystemNode Class:

Represents a node in the file system (a directory or a file).
Contains the name of the node, its content (if it's a file), and its children (if it's a directory).


Commit Class:

Represents a commit with a message, timestamp, and a snapshot of the file system at the time of the commit.


Branch Class:

Represents a branch with a name and a list of commits.
Provides a method to get the current snapshot of the file system.


Repository Class:

Represents a repository with a name, a root node of the file system, a map of branches, and the name of the current branch.
Provides methods to get the current branch.


Functions:

createRepository: Initializes a new repository.

commit: Commits changes to the repository.

createBranch: Creates a new branch.

switchBranch: Switches to a different branch.

mergeBranch: Merges changes from one branch to another and handles conflicts.

resolveConflict: Resolves conflicts by committing the provided resolution.

viewCommitHistory: Displays the commit history of a branch.

viewFileHistory: Displays the history of changes made to a specific file.


Driver Function:

Demonstrates the usage of the version control system by creating a repository, committing changes, creating and switching branches, merging branches, and viewing commit and file histories.

This implementation provides a basic version control system with functionalities similar to Git, focusing on hierarchical file organization, branching, merging, and viewing commit histories.
 main
