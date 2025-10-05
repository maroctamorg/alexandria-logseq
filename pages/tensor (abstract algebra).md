- #Algebra, #[[Riemannian Geometry]]
- [[idea]]
	- bilinear maps on a [[cartesian product]] $V \times X$ of [[vector space]]s $V$ and $W$ are in one-to-one correspondence with [[linear]] maps on the [[(set-)tensor product]].
- [[definition]]
	- Let $R$ be a [[commutative ring]] with [[identity]] and $V$ a left $R$[[-module]].
	  $B \subset V$ is called a [[(module-)basis]] if every $v \in V$ can be written uniquely as
	  $$v = \sum_i r_i bi_i$$
	  where $r_i \in R$ and $b_i \in B$.
		- An $R$ [[-module]] with a [[(module-)basis]] is said to be [[free]], and if $B$ is finite with n elements, then it is said to be of [[rank]] $n$.
	- The [[(set-)tensor product]] $V \otimes_R W$ of two $R$ [[-module]]s is the [[quotient]] $R$ [[-module]]
	  $$F(V \times W)/S$$
	  where
		- $F(V \times W)$, is the [[free]] $R$ [[-module]] with [[(module-)basis]] consisting of ordered pairs $(v, w) \in V \times W$.
		- $S$ is the [[submodule]] spanned by elements of the form
		  $$(v_1+v_2, w) - (v_1, w) - (v_2, w),$$
		  $$(v, w_1 + w_2) - (v, w_1) - (v, w_2),$$
		  $$(rv, w) - r(v, w),$$
		  $$(v, rw) - r(v, w),$$
		  where $v, v_i \in V, w, w_i \in W$ and $r \in R$.
	- The [[equivalence class]] of an element $(v, w)$ is denoted by $v \otimes w$ and called [[tensor product]] of $v$ and $w$.
		- An element in $V \otimes_R W$ of the form $v \otimes w$ is called a [[pure tensor]], and every element of the [[(set-)tensor product]] $V \otimes W$ is a finite sum of [[pure tensor]]s.
- [[theorem]]
	- [[tensor-universality]] Let $V, W$ and $Z$ be left $R$ [[-module]]s. Given any $R$-bilinear map $f : V \times W \to Z$, there **exists** a **unique** $R$-linear map $\tilde{f} : V \otimes W \to Z$ such that the following diagram [[commutes]]:
	  $$\begin{CD}
	       V \otimes W @= V \otimes W\\
	       @A \otimes AA @V \tilde{f} VV\\
	       V \times W @> f >> Z
	  \end{CD}$$