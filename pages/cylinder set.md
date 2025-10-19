- [[definition]]
  - For a finite or countable family $(\Omega_i,\mathcal{F}_i)$, a cylinder set is a measurable “finite-coordinate” set of the form
    $$ C=\Big(\prod_{i=1}^N A_i\Big)\times\Big(\prod_{i>N} \Omega_i\Big),\qquad A_i\in\mathcal{F}_i,\ N\in\mathbb{N}. $$
- [[generation]]
  - For fixed $N$, cylinders with $N$ specified coordinates form a $\pi$-system $\mathcal{C}_N$; the union $\mathcal{C}:=\bigcup_{N\ge1}\mathcal{C}_N$ generates the product $\sigma$-algebra on $\prod_i\Omega_i$.
  - On $\mathcal{C}$, define a pre-measure by $\mu(\prod_{i\le N}A_i\times\prod_{i>N}\Omega_i):=\prod_{i\le N}\mu_i(A_i)$; extend via [[Caratheodory extension theorem]].
- [[usage]]
  - Fundamental for defining [[countable product of probability spaces]] and proving uniqueness via [[Dynkin's theorem]].