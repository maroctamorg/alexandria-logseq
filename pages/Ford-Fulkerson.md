- #[[Design and Analysis of Algorithms]]
- [[problem]]
	- [[maximum flow]]
- [[idea]]
	- Given a feasible flow $f$, find another flow $f'$ s.t. **[[augmenting]]** $f$ with $f'$ increases the total flow.
	  $$(f \uparrow f')(u, v) =
	  \left\{
	  \begin{array}{cr}
	  f(u, v) + f'(u,v) - f'(v,u), & (u,v) \in E\\
	  0 & \text{otherwise}
	  \end{array}
	  \right\}$$
	- Flow $f'$ is found through the [[residual network]].
- [[lemma]]
	- Let $P$ be a simple s-t path in the [[residual network]] and define the [[bottleneck capacity]]:
	  $$c_f(P) = min_{(u,v) \in P} c_f(u, v)$$
	  (where $c_f$ is the capacity in the [[residual network]]).
	- Then
	  $$f_P(u,v) = \left\{
	  \begin{array}{cr}
	  c_f(P) & if (u,v) \in P \\
	  0 & \text{otherwise}
	  \end{array}
	  \right\}$$
	  is a [[flow]] in the [[residual network]], and $(f\uparrow f_P)$ on $G$ increases the flow by $c_f(P)$.
- [[algorithm]]
	- Start with a 0 flow $f$.
	- Repeat until flow $f$ does not improve anymore:
		- Find an s-t path $P$ in the [[residual network]] and [[augment]] $f$ with the bottleneck flow induced by $P$.
		- Path $P$ is called an [[augmenting path]].
- [[proof]]
	- [[definition]]
		- A [[cut]] $(S, T)$ of $G = (E, V)$ is a [[partition]] of $V$ into two sets $S$ and $T$ such that $s \in S$ and $t \in T$.
			- The [[capacity]] $c(S, T)$ of a [[cut]] is the sum of capacities of edges from $S$ to $T$.
			- The [[flow]] $f(S, T)$ of a [[cut]] is the sum of flows from edges of $S$ to edges of $T$.
	- [[lemma]]
		- $|f| = f(S, T)$ for any [[cut]] $(S, T)$ of $G$.
			- (idea: push the flow from the cut to the source by rewriting sums)
	- [[theorem]]
		- [[Max-flow min-cut theorem]] The following are equivalent:
			- $f$ is a [[maximum flow]],
			- $G_f$ contains no [[augmenting path]]s,
			- $|f| = c(S, T)$ for some [[cut]] of $G$
- [[analysis]]
	- Running time is $O(|f^*||E|)$, where $f^*$ is the maximum flow in a graph with integral capacities.
- [[remarks]]
	- if the [[capacity]] is 0, we don't even draw the [[arcs]] (directed edges)
	- [[residual network]]s are defined in such a way that eventually there are no s-t paths, as the [[residual network]] edges can have 0 capacity by either having 0 flow through the original graph in the opposite direction, or full flow (matching capacity) in the same direction
		- this is an intuition on why it converges
	-