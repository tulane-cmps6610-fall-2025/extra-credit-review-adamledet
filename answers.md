# CMPS 6610 Extra Credit Answers
  
In this extra credit assignment, we will test and review concepts you
   have learned since the midterm exam. Please add your written answers
   to `answers.md` which you can convert to a PDF using
   `convert.sh`. Alternatively, you may scan and upload written
   answers to a file named `answers.pdf`.



1. **Algorithmic Paradigms**
My favorite algorithmic paradigm is Greedy Algorithms. I feel as though Greedy algorithms are simple to understand: making a choice based on criteria and selecting it into a solution. It feels to-the-point, and it would then make sense that my favorite specific algorithm is Dijkstra's which was our prime example of a Greedy Algorithm (well, that and the fractional knapsack problem). I was a bit torn to include Divide and Conqueor algorithms, but I can become a bit frustrated with them when imagining the many recursions spread out throughout the problem--especially when actually putting the algorithm into code (though it is always beautiful when efficiently written and working).


2. **Divide and Conquer**
Divide and Conqueor problems must have the optimal substructure property. A divide and conqueor strategy breaks your problem into a number of subproblems before recombining them. Each subproblem must be an independently solvable portion of the problem or else it would yield and incorrect answer when broken apart and reassembled. The optimal substructure property, by definition, states that an optimal solution can be formed from optimal solutions of its subproblems.
Let us assume we have our divide and conqueor problem, P, and break it into to subproblems p1 and p2. If p1 or p2 is not optimal, then their combination into P will yield a non-optimal solution. The subproblems of a problem P, then, must have optimal substructure.

3. **Randomization**

- 3a. 
Our 'a' is O(n^2), and our E[X] is the expected value of Quicksort, nlogn; so according to Markov's inequality, the probability Quicksort does at least n^2 computations is at most nlogn/(n^2) which simplifies to log(n)/n.

- 3b.
nlogn/(((10^c)n)logn) = 1/(10^c)
The probability of larger quantities of work are significantly smaller than the probability of our expected average. This means that our 'concentration' for Quicksort is strong around our average and diminishes harshly as we deviate farther from it.

4. **Greedy Algorithms**
Let us assume that we have a schedule, S, that does not have its shortest job first. The first job adds its processing time to every other job's waiting time. If the first job's processing time was smaller, less time would logically be added to every other job's waiting time. It would, then, be optimal to have the shortest job first as that minimizes the total wait time.
Let us assume that there is an optimal schedule that does not have the shortest job first. This schedule currently adds its first job's processing time to n-1 other jobs. It would be more optimal to add less time to other jobs by placing the shorter job first as that job would add its time n-1 times, and the original first job would now only add its time to n-2 other jobs.


5. **Dynamic Programming**


6. **Graphs**
*I'm assuming that the largest weight 'edge' in the cycle cannot be in any MST.
Let us assume we have a MST that does contain the heaviest edge, e, of a cycle, c. If we remove e, we will split our tree into two subtrees that could be joined using any edge from cycle c. If we join the graph using an edge that isn't e, we will create a new MST that is smaller than our first MST which creates a contradiction. Therefore, wthe largest weight edge in any cycle cannot be contained in a minimum spanning tree.