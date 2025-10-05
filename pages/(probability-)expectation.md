- #[[Probability Theory]]
- [[definition]]
	- An **expectation** of a [[scalar random variable]] is the [[Lebesgue integral]] over a [[probability space]]
	  $$\mathbb{E}(X) = \int_{\Omega} Xd\mathbb{P}$$
- [[corollaries]]
	- We say that $X$ has an [[expectation]] (or that is exists), if the integral exists and is finite
	- The [[expectation]] satisfies (holds as a property of integration for arbitrary measure spaces)
		- [[(expectation-)linearity]] if $\alpha, \beta \in \R$, and $\mathbb{E}X, \mathbb{E}Y$ exist,
		  then $\mathbb{E}(\alpha X + \beta Y) = \alpha \mathbb{E}X + \beta \mathbb{E}Y$ exists
		- [[(expectation-)monotonicity]] if $X, Y$ are [[measurable map]]s
		  s.t. $0 \le X(\omega) \le Y(\omega) \forall \omega \in \Omega$, and $\mathbb{E}Y$ exists,
		  then $\mathbb{E}X \le \mathbb{E}Y$
	- [[(expectation-)monotone convergence theorem]] if $X_i \ge 0$ are [[measurable]] and $X_i \nearrow X$ [[almost surely]], then $\mathbb{E}X_i \to \mathbb{E}X$
		- this answers the key question of when we can **exchange the limit and the expectation**
	- The [[expectation]] satisfies the following useful inequalities
		- [[Cauchy-Schwartz]]
		  $$\mathbb{E}(XY) \le \sqrt{\mathbb{E}(X^2)} \cdot \sqrt{\mathbb{E}(Y^2)}$$
		- [[Hölder's inequality]] for $p, q > 0, \frac{1}{p}+\frac{1}{q} = 1$
		  $$\mathbb{E}(XY) \le (\mathbb{E}|X|^p)^{\frac{1}{p}}(\mathbb{E}|Y|^q)^{\frac{1}{q}}$$
		- [[Jensen's inequality]] if $f : \R \to \R$ is a [[convex function]] and $\mathbb{E}|X| < \infty, \mathbb{E}|f(X)| < \infty$
		  $$f(\mathbb{E}X) \le \mathbb{E}(f(x))$$
			- in particular $f = |\cdot|, f = (\cdot)^2$
		- [[Chebyshev]] for a non-negative [[random variable]] $X$ and $a > 0$, one has
		  $$\mathbb{P}(X \ge a) \le \frac{\mathbb{E}X}{a}$$
- [[lemma]]
	- [[Fatou]] If $X_n \ge 0$, then
	  $$\lim \inf \mathbb{E} X_n \ge \mathbb{E} \lim \inf X_n$$
- [[theorems]]
	- [[Lebesgue's dominated convergence theorem]]
		- if $X_i$ are [[scalar random variable]]s, $X_i \to X$ [[almost surely]]
		- and there exists a [[random variable]] $Y$ with $\mathbb{E}(|Y|) < \infty$ s. that $\forall i, |X_i| \le |Y|$ [[almost surely]]
		- then $\mathbb{E}X_i \to \mathbb{E}X$
	- [[bounded convergence theorem]]
		- if there exists some constant $C > 0$ s. that $|X_i| \le C, \forall i$, (and the [[measure]] is finite), then we can take $Y=C$ in the above theorem
- [[lemma]]
	- Let $f \ge 0$ be a [[measurable map]] on a [[measure space]] $(\Omega, \mathcal{F}, \mu)$.
	  Then $\mu '$ is a measure on $\mathcal{F}$
	  $$\mu '(A) := \int_A f d \mu = \int_{\Omega} (f \cdot I_A) d \mu$$
- [[definition]]
	- [[Radon-Nikodym derivative]]
- [[theorems]]
	- [[abstract change of variable theorem]]
		- Let $(\Omega_1, \mathcal{F}_1, \mathbb{P})$ be [[probability space]], $(\Omega_2, \mathcal{F}_2)$ a [[measurable space]], $X : \Omega_1 \to \Omega_2$ a [[random variable]] and $f : \Omega_2 \to \R$ a [[measurable map]].
		  Then,
		  $$\mathbb{E}(f \circ X) = \int_{\Omega_2} f d\mu_X,$$
		  where $\mu_X$ denotes the [[random variable distribution]] of $X$
	- [[differentiating an integral, real line]]
		- Let $I \subset \R$ be an open interval, and $(\Omega, \mathcal{F}, \mu)$ a [[measure space]].
		  Assume that a function $f : I \times \Omega \to \R$ satisfies the following $\forall x \in I$:
			- $\omega \to f(x, \omega)$ is [[integrable]]
			- the derivative $\partial _x f(x, \omega)$ of $x \to f(x, \omega)$ exists [[almost surely]]
			- there is a [[measurable map]] $h : \Omega \to \R_{\ge 0}$ s. that. $\int_{\Omega} h d\mu \le \infty$ and $|\partial_x f(x, \omega)| \le h(\omega)$ [[almost surely]]
		- Then $\forall x \in I$
		  $$\partial_x \int_{\Omega} f(x, \omega) d\mu(\omega) = \int_{\Omega} \partial_x f(x, \omega) d\mu(\omega)$$
- [[differentiating an integral, complex plane]]
	- Let $I \subset \mathbb{C}$ be an open set, and $(\Omega, \mathcal{F}, \mu)$ a [[measure space]].
	  Assume that a function $f : I \times \Omega \to \mathbb{C}$ satisfies the following $\forall z \in I$:
		- $\omega \to f(z, \omega)$ is [[integrable]]
		- the function, $z \to f(z, \omega)$ is [[almost surely]] [[analytic]] in $I$
		- there is a [[measurable map]] $h : \Omega \to \R_{\ge 0}$ s. that. $\int_{\Omega} h d\mu \le \infty$ and $|f(z, \omega)| \le h(\omega)$ [[almost surely]]
	- Then, the function $\psi(z) := \int_{\Omega} f(z, \omega) d\mu(\omega)$ is [[analytic]] in $I$, and
	  $$\forall n \in \N, z \in I : \frac{\partial^n}{\partial z^n} \psi(z) = \int_{\Omega} \frac{\partial^n}{\partial z^n} f(z, \omega) d\mu(\omega)$$