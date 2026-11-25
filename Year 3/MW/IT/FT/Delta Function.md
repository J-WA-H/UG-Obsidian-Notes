The delta function is an infinitely narrow Gaussian.
$$\delta(x)=\lim_{ \sigma \to 0 } \frac{1}{\sqrt{ 2\pi\sigma^2 }}e^{-x^2/2\sigma^2} .$$
$$\delta(x)=\begin{cases}
\infty & x=0 \\
0 & x\neq 0
\end{cases}.$$
Sifting property:
$$\int_{-\infty}^{\infty}\delta(x-a)f(x)=f(a).$$
$$\delta(-x)=\delta(x)$$
$$\delta(ax)=\frac{1}{|a|}\delta(x).$$
The $\delta$-function is differentiable:
$$\int_{-\infty}^{\infty}\delta'(x-a)f(a)dx=-f'(a).$$
Proof:
$$\int_{-\infty}^{\infty}\delta'(x-a)f(x)dx=\cancelto{0}{[\delta(x-a)f(x)]_{-\infty}^{\infty}}-\int_{-\infty}^{\infty}\delta(x-a)f'(x)dx=-f'(a)\;\square$$
The integral of $\delta(x)$ is the heavy side step function $\Theta(x)$.
$$\Theta(x)=\begin{cases}
1 & x\geq 0 \\
0 & x< 0
\end{cases}.$$
![[Pasted image 20250125114142.png]]
$$\Theta'(x)=\delta(x)$$
proof:
$$\int_{-\infty}^{\infty}\Theta'(x-a)f(x)dx=[\Theta(x-a)f)x]^{\infty}_{-\infty}-\int_{-\infty}^{\infty}\Theta(x-a)f'(x)dx=f(+\infty)-\int_{a}^{\infty}f'(x)dx$$
$$=f(+\infty)-[f(x)]^{\infty}_{a}=f(a)\;\square$$
The completeness relation:
$$\frac{1}{2\pi}\int_{-\infty}^{\infty}e^{ik(x-x')}dk=\delta(x-x')$$
$$\frac{1}{2\pi}\int_{-\infty}^{\infty}e^{ix(k-k')}dx=\delta(k-k').$$
The [[Fourier Transform]] of the delta function is
$$\mathcal{F}[\delta(x)](k)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}\delta(x)e^{-ikx}dx=\frac{1}{\sqrt{ 2\pi }}.$$
