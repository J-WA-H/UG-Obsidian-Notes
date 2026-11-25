A Gaussian is defined by
$$f(x)=ae^{-(x-b)^2/2c^2}.$$
Consider the case where $a=c=1$ and $b=0$, and take its [[Fourier Transform]]:
$$f(x)=e^{-\frac12x^2}.$$
$$\tilde{f}(k)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}f(x)e^{-ikx}dx=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}e^{-\frac12x^2}e^{-ikx}dx$$
$$=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}e^{-\frac12(x^2+2ikx)}dx=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}e^{-\frac 12(x+ik)^2}e^{-\frac 12k^2}dx$$
$$=\frac{e^{-\frac 12k^2}}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}e^{-\frac 12(x+ik)^2}dx.$$
Call
$$I=\int_{-\infty}^{\infty}e^{-\frac 12(x+ik)^2}dx.$$
Complexify the function to give
$$\oint_{\gamma}e^{-\frac 12(z+ik)^2}dz=0.$$
The integral is zero from [[Cauchy's theorem]]. Create the contour $\gamma$:
![[Pasted image 20250122104056.png]]
Split this contour into four,
$$\gamma=\gamma_{u}+\gamma_{d}+\gamma_{l}+\gamma_{r}$$
$$0=\left[ \int_{\gamma_{u}}+\int_{\gamma_{d}}+\int_{\gamma_{l}}+\int_{\gamma_{r}} \right]e^{-\frac 12(z+ik)^2}dz.$$
$\gamma_{u}$: Real axis so $z\to x$, $y=0$
$$\int_{R}^{-R}e^{-\frac 12(x+ik)^2}dx=-I\text{ for } r\to \infty.$$
$\gamma_{d}$: $z=z-ik$
$$\int_{-R}^{R}e^{-\frac 12 (x-ik+ik)}dx=\int_{-R}^{R}e^{-\frac{1}{2}x^2}dx=\sqrt{ 2\pi }$$
This is from the Gaussian integral
$$\int_{-\infty}^{\infty} e^{-\alpha x^2}=\sqrt{ \frac{\pi}{\alpha} }.$$
$\gamma_{l}$: $z=-R+iy$
$$\int_{0}^{-k}e^{-\frac 12 (-R+iy+ik)^2}idy\to 0 \text{ as } R\to \infty.$$
This same reasoning can be given for $\gamma_{r}$.
This gives
$$-I+\sqrt{ 2\pi }=0\implies I=\sqrt{ 2\pi }.$$
Plugging this back into the Fourier transform:
$$\tilde{f}(k)=\frac{e^{-\frac 12k^2}}{\sqrt{ 2\pi }}\sqrt{ 2\pi }$$
$$\implies \tilde{f}(k)=e^{-\frac 12 k^2}.$$
The Fourier transform of a Gaussian is a Gaussian.
