- #[[differential geometry]], #[[Riemannian Geometry]]
- [[definition]]
	- A [[tangent vector]] of a [[differentiable manifold]] $M$ at $p \in M$ is a mapping $v : C^\infty(p) \to \R$ that satisfies:
		- $v(af + bg) = av(f) + bv(g)$, $f,g \in C^\infty (p)$, $a,b \in \R$
		- $v(fg) = g(p)v(f) + f(p)v(g)$ ([[Leibniz rule]])
	- The **tangent space** at $p$ is the ($\R$-)[[linear vector space]] of [[tangent vector]]s at $p$, denoted $T_pM$ or $M_p$.
	- Let $(U, x)$ be a [[chart]] at $p$. We define a [[tangent vector]] $(\partial_i)_p$ at $p$ (and call it [[coordinate vector]]) as follows:
		- $$(\partial_i)_p f = \left(\frac{\partial}{\partial x^i}\right)_p f = D_i(f \circ x^{-1})(x(p))$$
		- $f \in C^\infty(p)$
	- Let $M^m$ and $N^n$ be [[differentiable manifold]]s and let $f : M \to N$ be a $C^\infty$ map.
	  The **tangent map** of $f$ at $p$ is a [[linear map]] $f_* : T_pM \to T_{f(p)}N$ defined by:
	  $$(f_*v)g=v(g \circ f), \forall g \in C^\infty(f(p)), v \in T_pM$$
		- maps a tangent space to another (vector to vector) in regards to a [[smooth (manifold) mapping]] (continuous transformation) - i.e. a push forward directional derivative, or a composite derivative
- [[remarks]]
	- $C^\infty (p)$ is the set of [[smooth (manifold) mapping]]s defined on some [[(topology-)neighborhood]] of $p$.
- [[conceptual-notes]]
	- As always, the main idea is to use the smooth/differentiable structure on the manifold to study the differential/smooth properties of the manifold via familiar tools from vector calculus in $\R^n$.
	- The [[tangent vector]] represents the [[directional derivative]] of a smooth real-valued function on a [[(topology-)neighborhood]] of a point on the [[differentiable manifold]] (i.e. how it changes along a given path through that point).
- [[lemma]]
	- If $f \in C^k(B), k \ge 1$, is a [[real-valued]] function in a [[(topology-)ball]] $B = B^n(0, r) \subset \R^n$, then there exist functions $g_i \in C^{k-1}(B), i \in {1..n}$ such that:
		- $g_i(0) = D_i f(0)$
		- $f(y)-f(0) = \sum_{i=1}^n y_ig_i(y)$
		- for all $y = (y_1, .., y_n) \in B$
- [[theorems]]
	- If $(U, x)$ is a [[chart]] at $p$ and $v \in T_pM$, then
	  $$v = \sum_{i=1}^n vx^i(\partial_i)_p$$
		- furthermore, the [[coordinate vector]]s form a [[basis]] of $T_pM$ and hence $\text{dim} T_pM = n$
	- Let $f : M \to N$ be $C^\infty$ and $p \in M$. Then $f$ is a [[local diffeomorphism]] at $p$ if and only if $f_{*p} : T_pM \to T_{f(p)}N$ is an [[isomorphism]].
		- [[proof]] via [[inverse function theorem]] (of $\R^n$)