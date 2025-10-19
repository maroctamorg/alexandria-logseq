- [[definitions]]
  - Almost surely (a.s.): $X_n\to X$ a.s. if $\mathbb{P}(\{\omega: X_n(\omega)\to X(\omega)\})=1$ (see [[almost surely]]).
  - In probability: $X_n\xrightarrow{\mathbb{P}}X$ if $\forall\varepsilon>0,\ \mathbb{P}(|X_n-X|>\varepsilon)\to0$.
  - In distribution: $X_n\xrightarrow{d}X$ if $F_{X_n}(x)\to F_X(x)$ at all continuity points of [[probability distribution function]] $F_X$.
  - In $L^p$ ($p\ge1$): $X_n\to X$ in $L^p$ if $\|X_n-X\|_p\to0$.

- [[implications]]
  - $L^p\ \Rightarrow\ \mathbb{P}$-convergence.
  - a.s. $\Rightarrow$ $\mathbb{P}$-convergence.
  - $\mathbb{P}$-convergence $\Rightarrow$ every subsequence has a.s. convergent further subsequence (to $X$).
  - Distributional convergence is equivalent to bounded-continuous test functions: $\mathbb{E}f(X_n)\to\mathbb{E}f(X)$ for all bounded continuous $f$ (Portmanteau direction).

- [[compactness/tightness]]
  - [[tightness]]: $\forall\varepsilon>0\ \exists M: \sup_n \mathbb{P}(|X_n|>M)<\varepsilon$.
  - [[Helly's selection theorem]]: tight c.d.f.s admit a subsequence converging pointwise at continuity points to a c.d.f.

- [[representation]]
  - [[Skorokhod representation theorem]]: if $X_n\xrightarrow{d}X$ on $\mathbb{R}$, then on some space $Y_n\to Y$ a.s. with $Y_n\stackrel{d}{=}X_n$, $Y\stackrel{d}{=}X$.

- [[notes]]
  - Right-continuity of $F_X$: $\mathbb{P}(X<x)=\lim_{y\uparrow x}F_X(y)$ (Solutions1).
  - For moment-based arguments and CF methods, see [[characteristic function]].