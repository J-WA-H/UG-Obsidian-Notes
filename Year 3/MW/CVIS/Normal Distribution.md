The Gaussian probability that a random variable $X$ is found in some interval $dX$ around $X$ is
$$P(X)=\frac{1}{(2\pi\sigma^2)^{1/2}}e^{ -\frac{(X-\mu)^2}{2\alpha^2} }dX.$$
$\mu$ is the mean, $\sigma$ is the standard deviation, and $\sigma^2$ is the variance.
![[Pasted image 20250322113019.png]]
Properties:
- Peaks at $\mu$
- Spreads out with $\sigma$
- $$\int_{-\infty}^{\infty}P(X)dX=1.$$
The nth moment is defined as
$$\langle X^{n} \rangle =\int_{-\infty}^{\infty}(X)^nP(X)dX$$
where $n\in \mathbb{N}$.
The first three moments define the properties of the normal distribution:
$$\langle X^{0} \rangle=1$$
$$\langle X^{1} \rangle =\mu$$
$$\langle X^2 \rangle =\sigma^2+\mu^2.$$
The probability that a Gaussian random variable is less then $X$ away from the mean is the error function:
$$\text{erf}(X)=\frac{2}{\sqrt{ \pi }}\int_{0}^{X}e^{ -X'^2 }dX'.$$
This is a finite Gaussian integral.
For large $X$:
$$\lim_{ X \to \infty }\text{erf(X)}=1. $$
This integrand can be expanded as a power series expansion and integrating each term gives the error function as a series expansion.