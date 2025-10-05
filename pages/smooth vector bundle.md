- #[[differential geometry]], #[[Riemannian Geometry]]
- [[definition]]
	- A [[smooth vector bundle]] of [[rank]] $k$ over $M$ is a pair $(E, \pi)$ where $E$ is a smooth manifold and $\pi : E \to M$ is a [[surjective]] [[smooth mapping]] ([[projection]]) such that:
		- $\forall p \in M$, $E_p = \pi^{-1}(p) \subset E$ is a $k$-dimensional real vector space (i.e. a [[fibre]] of $E$ over $p$);
		- $\forall p \in M$ there exist a [[(topology-)neighborhood]] $U \ni p$ and a [[diffeomorphism]] $\phi : \pi^{-1}U \to U \times R^k$ (i.e. a [[local trivialization]] of $E$ over $U$) such that the following diagram [[commutes]]
		  $$\begin{CD}
		       \pi^{-1}U @> \phi >> U \times R^k\\
		       @V \pi VV @V \pi_1 VV\\
		       U @= U
		  \end{CD}$$
			- (above $\pi_1$ is the standard projection, and $\phi|E_q : E_q \to \{q\} \times R^k$ is a [[linear]] [[isomorphism]] for every $q \in U$).
	- $E$ is called the [[total space]] and $M$ is called the [[(bundle-)base]] of the bundle.
	- If there is a [[local trivialization]] of $E$ over the whole manifold $M$, $\phi : \pi^{-1}M \to M \times R^k$, then $E$ is a [[trivial bundle]].
	- A [[section]] of $E$ is any map $\sigma: M \to E$ such that $\pi \circ \sigma = id : M \to M$.
		- A [[smooth section]] is a section that is a [[smooth mapping]].
		- [[Zero section]] is a map $\zeta : M \to E$ such that
		  $$\zeta(p) = 0 \in E_p, \forall p \in M$$
	- A [[local frame]] of $E$ over an [[(topology-)open]] set $U \subset M$ is a $k$-tuple of [[smooth section]]s of $E$ (over $U$) such that ($\sigma_1, ..., \sigma_k$ ($\sigma_1(p), ..., \sigma_k(p))$ is a [[basis]] of $E_p$ for all $p \in U$.
		- If $U = M$, $(\sigma_1, ..., \sigma_k)$ is called a [[global frame]].