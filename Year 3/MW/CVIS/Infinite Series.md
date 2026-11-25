Let $a_{n},\;n\in \mathbb{N}$ be a sequence of terms. Let $a_{i}\in \mathbb{R}$ then$$S_{n}=\sum_{i=0}^{n}a_{i}$$is a partial sum.

If $\lim_{ n \to \infty } a_{n}=0$ then the series converges to $S=\sum_{i=1}^{\infty}a_{i}$. Otherwise the series diverges.

For a converging series, for any $\varepsilon>0\;\exists \;n\in \mathbb{N},\;S\in \mathbb{R}$ s.t. $|S_{n}-S|<\varepsilon\;\forall \;n>n_{0}$.
This implies $\lim_{ n \to \infty }a_{n}=0$.
The inverse however is not true, for example the harmonic series.
$$a_{n}=\frac{1}{n},\;\lim_{ n \to \infty } \frac{1}{n}=0\text{ but }\sum_{n=1}^{\infty} \frac{1}{n} \text{ diverges}.$$
Example: Geometric series - each term is a ratio times the previous term.
$$a_{n}=ra_{n-1}=r^na_{0}.$$
$$\therefore \sum_{n=1}^{\infty}a_{n}=a_{0}\sum_{n=1}^{\infty}r^n.$$
This converges if $|r|<1$.
An example of a geometric series is
$$\sum_{n=0}^{\infty}x^n=\frac{1}{1-x}$$
for $|x|<1$.
Proof:
Sum the finite parts of the finite parts of the series and multiply by $(1-x)$.
$$\sum_{m=0}^{n}x^m(1-x)=(1-x)(1+x+x^2+x^3+\dots +x^n)$$
$$=(1+x+x^2+x^3+\dots+x^n)-(x+x^2+x^3+x^4+\dots+x^{n+1})$$
$$=1-x^{n+1}.$$
If $|x|<1$ then $\lim_{ n \to \infty }x^{n+1}=0$ so 
$$\lim_{ n \to \infty } \sum_{m=0}^{n}x^{m}(1-x)=\lim_{ n \to \infty } (1-x^{n+1})\implies \sum_{m=1}^{\infty} x^{m}(1-x)=1$$
$$\implies \sum_{m=0}^{\infty}x^m=\frac{1}{1-x}\;\square$$
Example: Riemann-zeta function
$$\zeta(p)=\sum_{n=1}^{\infty}n^{-p}.$$
This converges for $p>1$ and becomes the harmonic series for $p=1$.

Example: Telescopic series - $a_{n}=b_{n}-b_{n+1}$.
$$S_{n}=\sum_{n=0}^{N}a_{n}=a_{0}+a_{1}+a_{2}+\dots+a_{N}$$
$$=b_{0}\cancel{-b_{1}+b_{1}}\cancel{-b_{2}+b_{2}}\cancel{-b_{3}+\dots+b_N}-b_{N+1}.$$
This converges to $b_{0}$ if $b_{N+1}\to 0$ as $N\to \infty$ .
$$\sum_{n=1}^{\infty} \frac{1}{n(n+1)}=\sum_{n=1}^{\infty}\left( \frac{1}{n}-\frac{1}{n+1} \right)=\lim_{ n \to \infty } \left( 1-\frac{1}{2}+\frac{1}{2}-\frac{1}{3}+\frac{1}{3}-\frac{1}{4}+\dots+\frac{1}{n}-\frac{1}{n+1} \right)$$
$$=\lim_{ n \to \infty } \left( 1-\frac{1}{n+1} \right)=1.$$

