- [[measure theory]]
- [[definition]]
	- Given a [[measurable space]] $(\Omega, \mathcal{F})$, a function $\mu : \mathcal{F} \to \R_+ := {x \in [0, \infty]}$ is called a [[measure]] if
		- $\mu(\empty) = 0$
		- $\mu$ is [[countably additive]] (on [[disjoint]] sets)
- [[corollaries]]
	- [[lower continuity]]
		- A [[measure]] is lower continuous if and only if
		- Given $A_1 \subset A_2 \subset ..., A_i \in \mathcal{F}$
			- $\implies \mu(\bigcup_i A_i) = \lim_{i \to \infty} \mu(A_i)$
	- [[upper continuity]]
		- A [[measure]] is upper continuous if and only if
		- Given $A_1 \supset A_2 \supset ..., A_i \in \mathcal{F}, \mu(\Omega) < \infty$
			- $\implies \mu(\bigcap_i A_i) = \lim_{i \to \infty} \mu(A_i)$
- [[lemma]]
	- #lower-continuity-lemma
		- A [[measure]] is [[countably additive]] if and only if it is [[finitely additive]] and has [[lower continuity]]
	- #upper-continuity-lemma
		- A [[measure]] is [[countably additive]] if and only if it is [[finitely additive]] and has [[upper continuity]]
	- For any measure $\mu$, the following hold
		- [[monotonicity]] $A \subset B : A, B \in F \implies \mu(A) \le \mu(B)$
		- [[union bound]] $A_i \in \mathcal{F} \implies \mu(\bigcup_iA_i) \leq \sum_i \mu(A_i)$
			- [[monotonicity]] + [[countable additivity]]
	- #push-forward-lemma
		- Given a [[measurable space]] $(\Omega_1, \mathcal{F}_1)$, and a [[map]] $f : \Omega_1 \to \Omega_2$,
		  then the [[set]] containing subsets of $\Omega$ with [[measurable]] [[preimage]]
		  $$\mathcal{F}_1 \circ f^{-1} := \{A \in 2^{\Omega_2} : f^{-1}(A) \in \mathcal{F}_1\}$$
		  is a $\sigma$-algebra on $\Omega_2$.
		- #push-forward-measure
		  Moreover, if $\mu$ is a [[measure]] on $\mathcal{F}_1$, then $\mu \circ f^{-1}$, defined by
		  $$\mu \circ f^{-1}(A) = \mu(f^{-1}(A))$$
		  is a [[measure]] on $\mathcal{F}_1 \circ f^{-1}$
		- [[measurable map]]
- [[conceptual-notes]]
	- [[proof]] in [[measure theory]] often employs [[construction]] of [[disjoint]] sets
		- because [[countable additivity]] only applies to [[disjoint]] sets
	- all of these indexed [[sequences]] are indexed on the natural numbers and thus [[countable]]
		-
	-