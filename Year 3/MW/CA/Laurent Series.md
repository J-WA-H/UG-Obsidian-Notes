Definition: A function is meromorphic in $D$ if it is [analytic](Complex%20Differentiation.md)/holomorphic except at the [poles](Poles%20and%20residue%20Theorem.md) of the function.

[Taylor's theorem](Taylor%20Series.md) allowed us to approximate functions through a series expansion around a non-singular point Laurent series is a generalisation where the expansion is taken about a singular point.

Let $f(z)$ be analytic within $C_{1}<\lvert z-z_{0} \rvert<C_{2}$ and $f$ is undefined at $z_{0}$.
![[Pasted image 20250102161720.png]]
The Laurent series around this singular point is
$$f(z)=\sum_{n=-\infty}^\infty a_{n}(z-z_{0})^n=\sum_{n=-\infty}^{-1}a_n(z-z_{0})^n+\sum_{n=9}^\infty a_{n}(z-z_{0})^n$$
$$=\sum_{n=1}^\infty a_{-n}(z-z_{0})^{-n}+\sum_{n=0}^\infty a_{n}(z-z_{0})^n.$$
The left sum is known as the principal part and the right sum the analytic part.
$$a_{n}=\frac{1}{2\pi i} \oint_{C} \frac{f(z)}{(z-z_{0})^{n+1}}dz$$
$$a_{{-n}}=\frac{1}{2\pi i}\oint_{C}f(z)(z-z_{0})^{n-1}dz.$$
where $C$ is any closed curve in the annulus that encloses $z_{0}$.

The principal part represents the singular behaviour of $f(z)$ near $z=z_{0}$ and the analytic part converges in the regions where $f$ is analytic. 
If all $a_{-n}$ are zeros then $f$ has an analytic singularity.
If some $a_{-n}$ are non-zero then $f$ has a singularity at $z_{0}$ and the order of the pole is determined by the lowest non-zero $a_{=n}$.
If infinitely many $a_{-n}$ are non-zero then $f$ has an essential singularity at $a_{-n}$.

The analytic part converges on $\lvert z-z_{0} \rvert<C_{2}$ and the principal part converges on $\lvert z-z_{0} \rvert>C_{1}$, so the full Laurent series converges in the annulus.