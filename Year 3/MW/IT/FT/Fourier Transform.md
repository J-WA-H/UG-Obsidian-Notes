Definition: Consider a square integrable function $f:\mathbb{R}\to \mathbb{C}$, where
$$\int ^{\infty}_{-\infty}|f(x)|^2dx$$
is finite, and $\lim_{ x \to \infty }f(x)=0$.
The Fourier transform, $\tilde{f}(k)$, is given by
$$\tilde{f}(k)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}f(x)e^{-ikx}dx.$$
$\tilde{f}(k)$ is a complex function with real input $k$. $\tilde{f}(k)$ has an amplitude and a phase.

The inverse Fourier transform is given by
$$f(x)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}\tilde{f}(k)e^{ikx}dk.$$
Example: the wavefunction $\psi(x):\mathbb{R}\to \mathbb{C}$
By definition of a wavefunction, $\psi(x)$ is square integrable. We can rewrite $\psi(x)$ as
$$\psi(x)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}\tilde{\psi}(k)e^{ikx}dk.$$
This gives $\psi(x)$ as a decomposition of plane waves. The amplitude of these waves are given by $\tilde{\psi}(k)$, where $k$ is the wavevector.

Example: Sound wave
Sound waves are compressions of air, so can be described by the pressure as a function of time, $P(t):\mathbb{R}\to \mathbb{R}$.
In frequency space, it is given by $\tilde{P}(\omega)$.
$$P(t)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}\tilde{P}(\omega)e^{i\omega t}d\omega.$$
![[Pasted image 20250122102345.png]]
Sometimes we denote the Fourier transform as $\mathcal{F}[f(x)](k)=\tilde{f}(k)$. The inverse Fourier transform is denoted as $\mathcal{F}[\tilde{f}(k)](x)=f(x)$.
Sometimes it is defined without the normalisation constant $1/\sqrt{ 2\pi }$.
