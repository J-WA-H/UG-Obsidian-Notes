Ratio test:
	If $\exists\;\lim_{ n \to \infty } \left\lvert  \frac{a_{n+1}}{a_{n}}  \right\rvert<1$ then $S=\sum a_{n}$ converges.
	If $\lim_{ n \to \infty }>1$ then the series diverges.
	If $\lim_{ n \to \infty }=1$ then the test is inconclusive.

Comparison test:
	If $0\leq a_{n}\leq b_{n}$ $\forall$ $n\geq n_{0}$:
		- $\sum b_{n}$ converges $\implies \sum a_{n}$ converges
		- $\sum a_{n}$ diverges $\implies$ $\sum b_{n}$ diverges.

Integral test:
	If $f(x)$ is continuous and monotonically decreases for $x>x_{0}$ and $f(n)\geq a_{n}$ then
$$\int_{x_{0}}^{\infty}f(x)dx<\infty \implies \sum_{n=0}^{\infty}a_{n} \text{ converges}.$$
	Example: Show that $\sum_{n=1}^{\infty} \frac{1}{n^2}$ converges.
	$$S_{n}=\frac{1}{1}+\frac{1}{2^2}+\frac{1}{3^2}+\frac{1}{4^2}+\dots+\frac{1}{n^2}<1+\int_{1}^{n} \frac{1}{x^2}dx.$$
	This is true as the series sums over the rectangles which is smaller than the total area under the curve.
	![[Pasted image 20250308125202.png]]
	$$\therefore S_{n}<1+\int_{1}^{n} \frac{1}{x^2}dx$$
	Take $n\to \infty$,
$$S<1+\int_{1}^{\infty} \frac{1}{x^2}dx=1+\left[ -\frac{1}{x} \right]_{1}^{\infty}=2$$
	which converges. $\square$

Cauchy's nth root test:
	$a_{n}\geq 0\; \forall\; n$:
	- If $\lim_{ n \to \infty }a_{n}^{1/n}<1\implies \sum a_{n}$ converges
	- If $\lim_{ n \to \infty }a_{n}^{1/n}>1\implies \sum b_{n}$ diverges
	- If $\lim_{ n \to \infty }a_{n}^{1/n}=1$, it is inconclusive.

Condensation test:
	If $a_{n}>0$ and $a_{n+1}\leq a_{n}$,
	$$\implies \sum_{n=1}^{\infty}a_{n}\text{ converges }\iff \sum_{n=1}^{\infty}2^{k}a_{2^{k}}\text{ converges}.$$
	Schematic proof:
	$$S=a_{1}+a_{2}+a_{3}+a_{4}+a_{5}+a_{6}+a_{7}+a_{8}+\dots$$
	$a_{3}\leq a_{2}$, $a_{5},a_{6},a_{7},a_{8}\leq a_{4}$ so
$$S<a_{1}+a_{2}+a_{2}+4a_{4}+\dots=2^{0}a_{1}+2^{1}a_{2}+2^{2}a_{4}+\dots$$
	Thus if $\sum {2}^{k}a_{2^{k}}$ converges then $\sum a_{n}$ must converge as it is always smaller.
	Proof of the inverse:
	Let $\sum_{n=0}^{\infty}a_{n}$ be convergent.
	$$a_{1}+\frac{1}{2}\sum_{n=1}^{\infty}2^{n}a_{2^{n}}=a_{1}+a_{2}+2a_{4}+4a_{8}+\dots+2^{k-1}a_{2^{k}}$$
	$$\leq a_{1}+a_{2}+a_{3}+a_{4}+a_{5}+a_{6}+a_{7}+a_{8}+\dots+a_{2^{k}-1}+a_{2^{k}}\leq \sum_{n=0}^{\infty}a_{n}.$$
	$$\implies \frac{1}{2} \sum_{n=1}^{k}2^{n}a_{2^{n}}\leq \sum_{n=1}^{\infty}a_{n}-a_{1}.$$
	$$\frac{1}{2}\sum_{n=1}^{\infty}2^{n}a_{2^{n}}\leq \sum_{n=1}^{\infty}a_{n}- \frac{a_{1}}{2}$$
	$$\therefore \sum_{n=0}^{\infty}2^{n}a_{2^{n}}\text{ converges} \;\square$$
Alternating series test:
	Suppose $u_{n}\in \mathbb{R}$ and $u_{n}\geq 0$
	$u_{n}$ forms a decreasing sequence with $u_{n}\to 0$ as $n\to \infty$ then the alternating series.
	$$\sum_{n=1}^{\infty}(-1)^{n+1}u_{n}\text{ must converge}.$$
	Proof:
	$$S_{2n}=u_{1}-u_{2}+u_{3}-u_{4}+\dots-u_{2n}$$
	$$S_{2n+2}=u_{1}-u_{2}+u_{3}-\dots-u_{2n}+u_{2n+2}$$
	$$=S_{2n}+u_{2n+1}-u_{2n+2}$$
	$$u_{2n+1}>u_{2n+2}\implies S_{2n+2}>S_{2n}.$$
	$$S_{2n+2}<u_{1}\implies u_{1}>S_{2n+2}>S_{2n}$$
	$\implies$ the alternating series converges.