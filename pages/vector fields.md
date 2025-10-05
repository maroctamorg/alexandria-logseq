- #[[Riemannian Geometry]]
- [[definition]]
	- [[vector field]]
	- We say that [[vector field]]s $V^1, ..., V^n$ form a [[frame]] in $A$ (or [[local frame]])if $\forall p \in A$, the vectors $V^1_p, ..., V^n_p$ form a [[basis]] of $T_pM$.
		- In the case $A = M$, we say they form a [[global frame]].
		- Moreover, if $M$ admits a [[smooth]] [[global frame]], then $M$ is called [[parallelizable]].
		  Equivalently, $TM$ is a [[trivial bundle]].
	- Let $(U, x)$ be a [[chart]] and $(\partial_i)_p = (\frac{\partial}{\partial x^i})_p$, the corresponding [[coordinate vector]]s at $p \in U$. Then:
	  $$\partial_i : U \to TM, p \to (\partial_i)_p$$
	  are vector fields in $U$, and we call these [[coordinate vector fields]].
		- The [[frame]] formed by [[coordinate vector fields]] is called [[coordinate frame]], and we can write any [[vector field]] $V$ in $U$ as:
		  $$V_p = v^i(p)(\partial_i)_p, p \in U,$$
		  where $v^i : U \to \R$ are called [[component functions]] of $V$ with respect to the [[chart]].
	- If $V, W$ are [[smooth vector field]]s in an open set $A \subset M$, and $f \in C^\infty(p), p \in A$, then $Vf \in C^\infty(p)$, and so $W_p(Vf) \in \R$ is well-defined.
	  We denote the function $WVf : A \to \R, p \to W_p(Vf)$, and furthermore $(WV)_pf = W_p(Vf)$.
		- We define the [[Lie bracket]] of $V$ and $W$:
		  $$[V, W]_pf = V_p(Wf) - W_p(V, f), p \in A, f \in C^\infty(p)$$
- [[convention]]
	- [[Einstein summation convention]]
- [[lemma]]
	- Let $V$ be a [[vector field]] on $M$. The following are equivalent:
		- $V \in \mathcal{T}(M)$ (i.e. [[smooth vector field]]);
		- the [[component functions]] of $V$ with respect to **any** [[chart]] are [[smooth]];
		- if $U \subset M$ is [[(topology-)open]] and $f: U \to \R$ is [[smooth]], then the function $Vf : U \to \R, (Vf)(p) = V_pf$, is [[smooth]].
	- The [[Lie bracket]] satisfies:
		- [[bilinearity]]
		- [[antisymmetry]]
		- [[Jacobi identity]] ([[permutativity]])
		  $$[X, [Y, Z]] + [Y, [Z, X]] + [Z, [X, Y]] = 0$$
		- [[scalar-vector product rule]]
		  $$[fX, gY] = fg[X,Y]+f(Xg)Y - g(Yf)X$$
		  (note that this is a pointwise-product of smooth scalar function and vector field)
	- Let $(U, x)$ be a [[chart]] and $\partial_i$, the corresponding [[coordinate vector fields]]. Then:
	  $$[\partial_i, \partial_j] = 0, \forall i, j$$
	-
- [[theorem]]
	- Let $A \subset M$ be [[(topology-)open]] and $V, W \in \mathcal{T}(A)$. Then:
		- $[V, W]_p \in T_pM$;
		- $[V,W]$ \in $\mathcal{T}(A)$ and
		  $$[V,W]f = V(Wf) - W(Vf), f \in C^\infty(A)$$
		- if $v^i, w^i$ are the [[component functions]], with respect to a chart $x = (x^i)$, then:
		  $$[V,W] = (v^i \partial_i w^j - w^i\partial_i v^j)\partial_j$$
- [[remarks]]
	- [[coordinate vector fields]] are [[smooth]] by the second bullet point.
	- The "product" $(WV)_p$ is **not** a [[derivation]], so $(WV)_p is not a [[tangent vector]]: this is because the [[Leibniz rule]] does not hold.