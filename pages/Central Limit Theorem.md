- [[theorem]] (CLT)
  - If $X_i$ are i.i.d. with $\mathbb{E}X_1=\mu$, $\operatorname{Var}(X_1)=\sigma^2<\infty$, then
    $\frac{\sum_{i=1}^n X_i-n\mu}{\sigma\sqrt{n}} \xrightarrow{d} \mathcal{N}(0,1)$.
- [[hint]]
  - Expand $\varphi_{S_n/\sqrt{n}}(t)=\prod_i\varphi_{X_i}(t/\sqrt{n})$ and use Taylor at $0$; tightness + Lévy continuity theorem.
- [[notes]]
  - Differentiation under expectation near $0$ justified by local integrability (lecture Prop. on differentiating integrals).