- #[[measure theory]]
- [[theorem]] (Cavalieri for sets)
  - Let $(\Omega_1,\mathcal{F}_1,\mu_1)$ and $(\Omega_2,\mathcal{F}_2,\mu_2)$ be $\sigma$-finite measure spaces, and let $E\in \mathcal{F}_1\otimes\mathcal{F}_2$.
    - For $\mu_1$-a.e. $\omega_1\in\Omega_1$, the section $E_{\omega_1}:=\{\omega_2\in\Omega_2:(\omega_1,\omega_2)\in E\}\in\mathcal{F}_2$; likewise $E^{\omega_2}\in\mathcal{F}_1$ for $\mu_2$-a.e. $\omega_2$.
    - The maps $\omega_1\mapsto \mu_2(E_{\omega_1})$ and $\omega_2\mapsto \mu_1(E^{\omega_2})$ are measurable and
      $$ (\mu_1\otimes\mu_2)(E)=\int_{\Omega_1} \mu_2(E_{\omega_1})\,d\mu_1(\omega_1)=\int_{\Omega_2} \mu_1(E^{\omega_2})\,d\mu_2(\omega_2). $$

- [[theorem]] (Cavalieri for nonnegative functions)
  - If $f\ge0$ is $(\mathcal{F}_1\otimes\mathcal{F}_2)$-measurable, then for $\mu_1$-a.e. $\omega_1$, the section $f_{\omega_1}(\cdot):=f(\omega_1,\cdot)$ is $\mathcal{F}_2$-measurable (and symmetrically), and
    $$ \int f\,d(\mu_1\otimes\mu_2)=\int\Big(\int f(\omega_1,\omega_2)\,d\mu_2(\omega_2)\Big)\,d\mu_1(\omega_1)=\int\Big(\int f\,d\mu_1\Big)\,d\mu_2. $$

- [[notes]]
  - On completed spaces, statements hold with sections/measurability understood a.e. w.r.t. the completion (see [[null-set]] caveat).
  - Intuition: measure by slices in either coordinate; the totals coincide.
  - For signed/integrable $f$, combine with [[Tonelli's theorem]] (for $f_+,f_-$) and [[Fubini's theorem]].

- [[see-also]] [[product measure]], [[Fubini's theorem]], [[Tonelli's theorem]]