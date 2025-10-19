- [[theorem]] (Chernoff/Hoeffding-style bound)
  - If $X_i$ are i.i.d., centered, and $\exists\,\theta>0$ with $\mathbb{E}e^{\theta X_1}<\infty$, then for $\varepsilon>0$,
    $\mathbb{P}(\bar{X}_n\ge \varepsilon)\le \exp\{-n\sup_{\lambda\in(0,\theta]}(\lambda\varepsilon-\log\mathbb{E}e^{\lambda X_1})\}$.
- [[concepts]]
  - [[moment generating function]] $\phi(\lambda)=\log\mathbb{E}e^{\lambda X}$ convex; optimize Markov bound.
- [[tips]] (Solutions4)
  - Interchange of expectation/derivatives justified by dominated convergence (differentiate under the integral when locally bounded). Use Tonelli/Fubini carefully; absolute integrability needed for Fubini.