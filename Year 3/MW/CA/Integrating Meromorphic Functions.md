Let $f$ be [analytic](Complex%20Differentiation.md) within an annulus bounded by $C_{1}<\lvert z-z_{0} \rvert<C_{2}$. Let $C$ be a closed curve contained in the annulus encircling $z_{0}$.
$$f(z)=\sum_{n=0}^\infty a_{n}(z-z_{0})^n+\sum_{n=-\infty}^{-1}a_{n}(z-z_{0})^n$$from the [Laurent series](Laurent%20Series.md). Integrating this gives
$$\oint_{C}f(z)dz=\cancelto{0}{\oint_{C}\sum_{n=0}^\infty a_{n}(z-z_{0})^ndz}+\oint_{C}\sum_{n=-\infty}^{-1}a_{n}(z-z_{0})^ndz.$$
The integral of the analytic part over $C$ goes to zero from [[Cauchy's theorem]] so only the principal part is left.

Aside:
$$\oint_{C}\frac{dz}{z^n}$$
Use Cauchy's integral formula:
$$\oint_{C} \frac{1}{z^n}dz= 2\pi if^{(n-1)}(0)$$
$f(z)=1$ so for $n>1$, this integral goes to zero, so the only term that survives is $n=1$, for which the integral is $2\pi i$.

$$\oint_{C}f(z)dz=\oint_{C}\sum_{n=-\infty}^{-1}a_{n}(z-z_{0})^ndz.$$
From the above, the only term in the sum that does not go to zero is $n=-1$. This simplifies the integral to
$$\oint_{C}f(z)dz=\oint_{C}a_{{-1}}(z-z_{0})^{-1}dz=2\pi ia_{-1}.$$
$a_{-1}$ is known as the residue.
