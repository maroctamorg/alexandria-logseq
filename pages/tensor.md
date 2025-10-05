- #[[differential geometry]], #[[Riemannian Geometry]]
- [[definition]]
	- A [[tensor]] is a [[multi-linear]] map on a finite product of a [[vector space]] and its [[dual]].
		- A $k$-[[covariant]] [[tensor]] on $V$ is a $k$-linear map
		  $$V^k \to \R, V^k = V \times ... \times V$$
			- we denote their space $T^k(V)$
		- An $l$-[[contravariant]] [[tensor]] on $V$ is an $l$-linear map
		  $$V^{*l} \to \R, V^{*l} = V^* \times ... \times V^*$$
			- we denote their space $T_l(V)$
		- A $k$-[[covariant]], $l$-[[contravariant]] [[tensor]] (or a $(k, l)$-[[tensor]]) on $V$ is a $(k+l)$-linear map
		  $$V^k \times V^{*l} \to \R$$
			- we denote their space $T^k_l(V)$
	- The [[tensor product]] of [[tensor]]s $F \in T^k_l(V)$ and $G \in T^p_q(V)$ is the [[tensor]] $F \otimes G \in T^{k+p}_{l+q}$,
	  $$F \otimes G(v_1, ..., V_{k+p}, \omega^1, ..., \omega^{l+q}) = F(v_1, ..., v_k, \omega^1, ..., \omega^l)G(v_{k+1}, ..., v_{k+p}, \omega^{l+1}, ..., \omega^{l+q}).$$
- [[convention]]
	- $T^0(V) = T_0(V) = T^0_0(V) = \R$
- [[lemma]]
	- If $(v_i)$ is a [[basis]] of $V$ and $(\omega^j)$ the corresponding [[dual basis]] of $V^*$, then the tensors
	  $$\omega^{i_1} \otimes ... \otimes \omega^{i_k} \otimes v_{j_1} \otimes ... \otimes v_{j_l} \in T^k_l(V)$$
	  form a [[basis]] of $T^k_l(V)$.
		- Consequently, $\text{dim}T^k_l(V) = n^{k+l}$.
- [[remarks]]
	- These spaces are [[vector space]]s in a natural way.
	- [[covector]]s are 1-[[covariant]] [[tensor]]s.