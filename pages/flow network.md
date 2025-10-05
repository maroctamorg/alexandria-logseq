- #[[Design and Analysis of Algorithms]]
- [[definition]]
	- Let $G = (V, E)$ be a [[directed graph]] with no parallel edges. We say that $G$ equipped with functions $f, g : E \to \R^+$, named [[flow]] and [[capacity]] respectively, is a **flow network** if it satisfies:
		- $\forall (u, v) \in E, f(u, v) \le c(u, v)$
		- [[flow conservation]], i.e. flow coming in equals flow coming out
		  $$\sum_{(u, v) \in E} f(u, v) = \sum_{(v, w)\in E} f(v, w)$$
			- $\forall v \in E$, except for two special nodes $s$ ([[source]]) and $t$ (target or [[sink]]) where we define the [[total flow]]
			  $$|f| = \sum_{(s, v) \in E} f(s,v) = \sum_{(w, t) \in E} f(w,t)$$
				- these two special nodes have the unique properties
					- $N^-(s) := \{(u, s) \in E\} = \empty$
					- $N^+(t) := \{(t, v) \in E\} = \empty$
	- The [[residual network]] of $G$ is denoted $G_f = (V, E_f)$, and is defined by taking each edge $(u, v) \in E$ and
		- adding $(u, v)$ to $E_f$ with [[capacity]] $c(u, v) - f(u, v)$
		- adding $(v, u)$ to $E_f$ with [[capacity]] $f(u, v)$