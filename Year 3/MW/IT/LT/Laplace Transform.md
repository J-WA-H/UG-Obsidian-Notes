The Laplace transform is an integral transform for functions that are not [square integrable](Fourier%20Transform.md) and if we have boundary conditions.

Consider a function $f(t):\mathbb{R}\to \mathbb{C}$ and $f(t<0)=0$, then $f$ is locally integrable on $t\in[0,\infty)$. The Laplace transform is given by
$$\hat{f}(s)=\mathcal{L}[f(t)](s)=\int_{0}^{\infty}dte^{-st}f(t)$$
where $s>0$ and complex, $s=\sigma+i\omega;\;\sigma,\omega\in \mathbb{R}$.

$f(t)$ can diverge for $t\to \infty$ but there must be some variable $s>0$ s.t. 
$$\lim_{ t \to \infty } f(t)e^{-st}=0.$$
The Laplace transform of $f(t)$ is equivalent to the Laplace transform of $f(t)\Theta(t)$, the [heavy side function](Delta%20Function.md).

Examples:
$$\mathcal{L}[\Theta(t)](s)=\int_{0}^{\infty}dte^{-st}\Theta(t)=\int_{0}^{\infty}dte^{-st}=\left[ -\frac{e^{-st}}{s} \right]_{0}^{\infty}=\frac{1}{s}.$$
$$\mathcal{L}[e^{\lambda t}](s)=\int_{0}^{\infty}dte^{-st}e^{\lambda t}=\int_{0}^{\infty}dte^{-t(s-\lambda)}=\left[ \frac{1}{s-\lambda}e^{-t(s-\lambda)} \right]_{0}^{\infty}=\frac{1}{s-\lambda}$$
for $s>\mathrm{Re}[\lambda]$.
$$\mathcal{L}[\sin t](s)=\int_{0}^{\infty}dte^{-st}\sin t=\frac{1}{2i}\int_{0}^{\infty}e^{-st}(e^{it}-e^{-it})dt=\frac{1}{2i}\int_{0}^{\infty}e^{-t(s-i)}-e^{-t(s+i)}dt$$
$$=\frac{1}{2i}\left[ -\frac{1}{s-i}e^{-t(s-i)}+\frac{1}{s+i}e^{-t(s+i)} \right]_{0}^{\infty}=\frac{1}{2i}\left( \frac{1}{s-i}-\frac{1}{s+i} \right)=\frac{1}{2i} \frac{{s+i-s+i}}{(s+i)(s-i)}$$
$$=\frac{1}{2i} \frac{2i}{s^2+1}=\frac{1}{s^2+1}.$$
