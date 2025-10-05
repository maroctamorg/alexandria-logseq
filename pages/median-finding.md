- #[[Design and Analysis of Algorithms]], #recurrence, #divide-and-conquer
- [[idea]]
	- **key**: assume the linear-time algorithm exists and use it to solve a more generic problem,
	  then prove the algorithm can be substituted by an approximation which is satisfies linear time for the application of the generic algorithm to the specific problem
		- here the generic algorithm is selecting the $j$-th smallest value in an array
		- the approximation is to take the median of medians of blocks of length $\lceil n/5 \rceil$
-