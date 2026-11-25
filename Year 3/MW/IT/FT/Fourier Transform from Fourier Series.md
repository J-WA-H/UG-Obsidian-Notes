For a periodic function of period $L$, the Fourier series is given by
$$f(x)=\sum_{n=-\infty}^{\infty}c_{n}e^{i2\pi nx/L}$$
where
$$c_{n}=\frac{1}{L}\int_{-L/2}^{L/2}f(x)e^{-i2\pi nx/L}dx.$$
To get the Fourier transform we need $f$ to be continuous and differentiable in $\left[ -\frac{L}{2}, \frac{L}{2} \right]$.
Start with $k=\frac{2\pi n}{L}$, $\delta n=1$
$$f(x)=\sum_{n}\delta nc_{n}e^{ikx}.$$
$$\frac{\delta k}{\delta n}=\frac{2\pi}{L}\implies\delta n=1=\delta k \frac{L}{2\pi}$$
$$f(x)=\frac{L}{2\pi}\sum_{k=-\infty}^{\infty}\delta k c_{n}e^{ikx}=\frac{L}{2\pi}\sum_{k}\delta k\left( \frac{1}{L}\int_{-L/2}^{L/2}f(x')e^{-ikx'}dx' \right)e^{ikx}$$
$$=\frac{1}{\sqrt{ 2\pi }}\sum_{k}\delta k\left( \frac{1}{\sqrt{ 2\pi }} \int_{-L/2}^{L/2}f(x')e^{-ikx'}dx' \right)e^{ikx}$$
Take $L\to \infty \implies \sum_{k}\to \int dk$:
$$f(x)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dk\left( \frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}f(x')e^{-ikx'}dx' \right)e^{ikx}$$
$$f(x)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}\tilde{f}(k)e^{ikx}dk$$
Rearranging gives
$$f(x)=\int_{-\infty}^{\infty}dx'\left[ f(x')\left( \frac{1}{2\pi}\int_{-\infty}^{\infty}dke^{ik(x-x')} \right) \right]$$
$$f(x)=\int ^{\infty}_{-\infty}dx'f(x')\delta(x-x').$$
$$\therefore \frac{1}{2\pi}\int_{-\infty}^{\infty}dke^{ik(x-x')}=\delta(x-x').$$
