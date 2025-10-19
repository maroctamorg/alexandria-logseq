- #[[measure theory]]
- [[theorem]] (Fubini)
  - Let $(\Omega_i,\mathcal{F}_i,\mu_i)$ be complete $\sigma$-finite measure spaces and $f\in L^1(\mu_1\otimes\mu_2)$.
    Then for $\mu_1$-a.e. $\omega_1$ and $\mu_2$-a.e. $\omega_2$, the sections $f(\omega_1,\cdot)\in L^1(\mu_2)$ and $f(\cdot,\omega_2)\in L^1(\mu_1)$, and
    $$ \int f\,d(\mu_1\otimes\mu_2)=\int\Big(\int f(\omega_1,\omega_2)\,d\mu_2(\omega_2)\Big)\,d\mu_1(\omega_1)=\int\Big(\int f\,d\mu_1\Big)\,d\mu_2. $$

- [[notes]]
  - Requires [[absolute integrability]]: $\int |f|\,d(\mu_1\otimes\mu_2)<\infty$. Without it, use [[Tonelli's theorem]] for $f\ge0$ (or apply to $f_+,f_-$).
  - Ensures the two iterated integrals exist and are equal to the product integral; order of integration can be swapped.
  - See also [[product measure]] and [[Cavalieri principle]].