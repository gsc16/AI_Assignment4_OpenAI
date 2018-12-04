# Breadth First Search:
In this traversing algorithm, we use the strategy to expand a shallowest node first. 
We start with the root of the graph and traverse all the nodes at the current depth before going to the next depth level.
This is implemented using a FIFO queue.
It is optimal only if the node to be searched is the node at the first level.

# Depth First Search:
In this traversing algorithm, we use the strategy to expand a deepest node first. 
We start with the root and explore as far as possible along each branch. This is implemented using a LIFO stack.
It is optimal only if the node to be searched is the left-most node.

# Uniform Cost Search:
In this traversing algorithm, we use the strategy to expand a cheapest node first. 
This is implemented using a priority queue and nodes are traversed base don the priority. 
It is optimal as it considers the path with the low cost.

# Greedy search:
In this traversing algorithm, we traverse the closest node first. 
This is not optimal as there might be paths that have low cost compared to the path taken.

# A* Search:
This algorithm uses both Uniform Cost search and Greedy search. 
It uses both the backward costs and the estimates of the forward costs. Hence, it is optimal and admissible.


# Minimax:
This is a recursive algorithm used for adversarial search. A value is associated with each position or state. 
This value is determined by an evaluation fucntion which computes the maximizes the value of the minimum agent and minimizes the value of 
maximum agent. Usually, minimum agent is Pacman and Maximum agent is Ghost, in case of Pacman game.

# Expectimax search:
Expectimax search is a variation of Minimax search, where max nodes are computed same as in Minimax search. 
Chance nodes are like min nodes in Minimax, but their outcomes are uncertain. So, we calculate the weighted average values of the children.

# Alpha-beta pruning:
It is an adversarial search algorithm that decreases the number of nodes that are evaluated by the minimax algorithm. 
It stops evaluating when at least one best move is found.
