- #[[differential geometry]], #[[Riemannian Geometry]]
- [[definition]]
	- We define the **tangent bundle** $TM$ of a [[differentiable manifold]] $M$ as a [[disjoint]] union of all [[tangent space]]s of $M$, i.e.
	  $$TM = \bigcup_{p \in M} (p, T_pM)$$
	- Let $\pi: TM \to M$ be the [[projection]] ($\pi(v) = \pi(p, v) = p \in M$ for $p \in T_pM$).
	  Then $\pi^{-1}(p) = T_pM$ is a [[fibre]] over $p$.
		- a fibre is the set, not the map - the inverse in fact is not a map here
	- A map $s : A \subset M \to TM$, with $\pi \circ s = id$, is a [[section]] of $TM$ in $A$ (or a [[vector field]]).
		- a section assigns to each point, a vector in its corresponding tangent space
	- [[smooth vector bundle]]
- [[theorem]]
	- Let $M$ be a [[differentiable manifold]] of dimension $n$. The [[tangent bundle]] $TM$ of $M$ can be equipped with a natural [[topology]] and a $C^\infty$-structure of a [[differentiable manifold]] of dimension $2n$ such that the projection $\pi : TM \to M$ is a [[smooth (manifold) mapping]].
-