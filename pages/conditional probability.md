- If $(\Omega, \mathcal{F}, \mathbb{P})$ is a [[probability space]], and $A \in \mathcal{F}$, then the #restriction $\mathcal{F}|_A := \{A \cap B : B \in \mathcal{F}\}$ is a [[sigma-algebra]] on $A$ and $\mu(B) := \mathbb(A \cap B)$ is a measure on $\mathcal{F}|_A$
	- If $\mathbb{P}(A) = 0$, then this [[measure]] is always identically zero, otherwise we can normalize it to be a [[probability measure]] on $A$ and this is called ***conditional probability*** denoted $\mathbb{P}(\circ | A)$ and defined as
	  $$\mathbb{P}(B|A)=\frac{\mathbb{P}(B \cap A)}{\mathbb{P}(A)}$$
		- exchanging $A$ and $B$ above, we arrive at *[[Baye's formula]]*
-