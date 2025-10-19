- #[[measure theory]]
- [[theorem]] (Tonelli)
  - Let $(\Omega_i,\mathcal{F}_i,\mu_i)$ be complete $\sigma$-finite measure spaces and $f\ge0$ be $(\mathcal{F}_1\otimes\mathcal{F}_2)$-measurable. Then
    $$ \int f\,d(\mu_1\otimes\mu_2)=\int\Big(\int f(\omega_1,\omega_2)\,d\mu_2(\omega_2)\Big)\,d\mu_1(\omega_1)=\int\Big(\int f\,d\mu_1\Big)\,d\mu_2, $$
    with all integrals in $[0,\infty]$.

- [[notes]]
  - No [[absolute integrability]] assumption needed; apply to $f_+,f_-$ to reduce Fubini to Tonelli.
  - See also [[Cavalieri principle]] for sets and indicator functions; [[product measure]].