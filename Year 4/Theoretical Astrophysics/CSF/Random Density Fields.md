3In the early universe $\delta(\vec{x},t)$ is a random field so it needs a statistical description. Solutions have [plane wave solutions](Perturbations%20with%20Pressure.md) $\delta(\vec{x},t)=\delta_{\vec{k}}(t)e^{ i\vec{k}\cdot \vec{x} }$. Fourier theorem implies the general density field as a sum of plane waves,
$$\delta(\vec{x},t)=\sum_{\vec{k}}\delta_{\vec{k}}(t)e^{ i\vec{k}\cdot \vec{x} }.\tag{21.1} $$
In linear perturbation theory, each $\delta_{\vec{k}}$ evolves independently of the other when $\delta$ is small. The complex amplitudes $\delta_{\vec{k}}$ are random numbers with $\langle \delta_{\vec{k}} \rangle=0$. $\langle |\delta_{\vec{k}}|^2 \rangle$ is the power spectrum up to a factor $V$ with $\langle |\delta_{\vec{k}}|^2 \rangle\geq 0$.
![[Pasted image 20251123110711.png]]
For a field $\delta(\vec{x},t)$ in comoving coordinates, the Fourier transform implies
$$\delta_{\vec{k}}(\vec{k},t)=\int\delta(\vec{x},t)e^{ -i\vec{k}\cdot \vec{x} }\;d^3x\tag{21.2} $$
$$\delta(\vec{x},t)=\frac{1}{(2\pi)^3}\int \delta_{k}(\vec{k},t)e^{ i\vec{k}\cdot \vec{x} }\;d^3k\tag{21.3} .$$
$\delta_{k}(\vec{k},t)$ is in general complex but $\delta ^{*}_{k}(\vec{k},t)=\delta_{k}(-\vec{k},t)$ since $\delta(\vec{x},t)\in \mathbb{R}$. In practice, $\int d^3x$ is over a large volume $V$ as all space is difficult to work with. This gives the power spectrum
$$P(\vec{k})\equiv \frac{{\langle |\delta_{k}(\vec{k})|^2 \rangle }}{V}\tag{21.4} .$$
For a random field, $|\delta_{k}(\vec{k})|^2$ fluctuates rapidly with $k$ as independent plane waves but $\langle |\delta_{k}(\vec{k})|^2 \rangle$ is normally a smoothly varying quantity.

For a Gaussian random field, complex amplitudes $\delta_{k}$ are drawn from a Gaussian probability distribution with $\langle \delta_{k} \rangle=0$. The statistical properties of $\delta(\vec{x})$ are completely satisfied by $P(\vec{k})$. $\delta(\vec{x})$ is usually assumed to be statistically isotropic so $P(\vec{k})=P(k)$, it depends on the magnitude of $k=|\vec{k}|$ but not the direction.

For a Gaussian random field with $\langle \delta \rangle=0$, the probability distribution for $\delta(\vec{x})$ at any point is Gaussian with dispersion $\sigma$,
$$p(\delta)d\delta=\frac{1}{\sqrt{ 2\pi }\sigma}e^{ -\delta^2/2\sigma^2 }.\tag{21.5} $$
This implies $\delta$ is equally likely to be overdense ($\delta>0$) or underdense ($\delta<0$) with a typical $|\delta|\sim \sigma$. 

In cosmology, the evolution of $\delta_{k}$ with time is in general a sum of growing and decaying modes,
$$\delta_{k}(\vec{k},t)=A_{\vec{k}}D_{+}(k,t)+B_{\vec{k}}D_{-}(k,t).\tag{21.6} $$
For simplicity, only consider growing mode perturbations. Then $P(k,t)\propto \langle |\delta_{k}(\vec{k},t)|^2 \rangle\propto |D_{+}(k,t)|^2$. Hence the evolution of the power spectrum between time $t_{i}$ and $t_{f}$ to
$$P(k,t_{f})=\left\lvert  \frac{D_{+}(k,t_{f})}{D_{+}(k,t_{i})}  \right\rvert ^2P(k,t_{i})\tag{21.7} .$$
$P(k,t)$ can evolve in shape and amplitude as $D_{+}(k,t)$ in general depends on $k$. From non-linear evolution, dark matter halos typically form roughly spherical regions of the initial density field, which collapse due to its own self-gravity. From linear perturbation theory, spherical perturbations of radius $R$ collapses when
$$\left( \frac{\delta \rho}{\bar{\rho}} \right)_{E}\simeq 1\tag{21.8} $$
where $\left( \frac{\delta \rho}{\bar{\rho}} \right)_{R}\equiv\delta^{(R)}$ is the mean value of $\frac{\delta \rho}{\bar{\rho}}$ within a sphere of radius $R$.

Consider averaging $\delta(x)$ over different spheres of radius $R$. For a sphere centred at $\vec{x}=0$,
$$\delta^{(R)}(\vec{x}=0)=\frac{1}{\frac{4}{3}\pi R^3}\int_{|\vec{x}|<R}\delta(\vec{x})d^3x.\tag{21.9} $$
The average of $\delta$ in a sphere of radius $R$ placed around an arbitrary point $\vec{x}$ is a convolution
$$\delta^{(R)}(\vec{x})=\delta*W(\vec{x})\equiv\int \delta(\vec{y})W(\vec{x}-\vec{y};R)d^3y\tag{21.10} $$where $W(\vec{x};R)$ is a window function of radius $R$. We will take $W(\vec{x};R)$ as a spherical top hat window function
$$W(\vec{x};R)=\begin{cases}
\frac{1}{\frac{4}{3}\pi R^3} & |\vec{x}|<R \\
0 & \text{otherwise}
\end{cases}.\tag{21.11} $$
This is normalised such that
$$\int W(\vec{x};R)d^3x=1.\tag{21.12} $$
Note that more general window functions exist.

$\delta^{(R)}(\vec{x})$ is a smoother out version of the original density field $\delta(\vec{x})$. If $\delta^{(R)}(\vec{x},t)\gtrsim 1$ then the region of radius $R$ around the point $\vec{x}$ undergoes gravitational collapse by time $t$. Measuring $\delta^{(R)}$ around different points gives the probability distribution of $\delta^{(R)}$. The Gaussian random field gives $P(\delta^{(R)})$ also Gaussian with a mean $\langle \delta^{(R)} \rangle$ and dispersion $\sigma(R)$. The average over a large volume gives
$$\langle \delta^{(R)} \rangle \equiv \frac{{1}}{V}\int d^3x\;\delta^{(R)}(\vec{x})=0.\tag{21.13} $$
The variance is hence defined as
$$\sigma^2(R)=\langle (\delta^{(R)})^2 \rangle \equiv \frac{1}{V}\int d^3x(\delta^{(R)}(\vec{x}))^2=\frac{1}{(2\pi)^3}\int {\frac{|\delta^{(R)}_{k}(\vec{k})|^2}{V}}d^3k.\tag{21.14} $$This result uses Parseval's theorem. One can then show that
$$\sigma^{2}(R)=\frac{1}{(2\pi)^3}\int d^3k|W_{k}(\vec{k};R)|^2P(k)\tag{21.15} $$where $W_{k}(\vec{k};R)$ is the Fourier transform of the window function.

For a uniform spherical window,
$$W_{k}(\vec{k};R)=W_{k}(k;R)=3 \frac{{\sin(KR)-KR\cos(KR)}}{(KR)^3}.\tag{21.16} $$
Thus for an isotropic $P(k)$,
$$\sigma^2(R)=\frac{1}{(2\pi)^3}\int_{0}^{\infty} |W_{k}(k;R)|^2P(k)4\pi k^2dk.\tag{21.17} $$
![[Pasted image 20251123125955.png]]
The general trend is
$$W_{k}(k;R)=\begin{cases}
1 & KR\ll 1 \\
0 & KR\gg 0
\end{cases}.\tag{21.18} $$
Here $W_{k}\sim \frac{1}{(KR)^2}$ for $KR\gg 1$.

The contributions to $\sigma^2$ for large k from $W_{k}$ is suppressed so $W_{k}$ acts on $P(k)$ as a low-pass filter.
![[Pasted image 20251123130322.png]]
Note that $P=P(k,t)$ gives $\sigma=\sigma(R,t)$ with $k,R$ in comoving coordinates.

$\sigma(R,t)$ is the RMS value of $\frac{\delta \rho}{\bar{\rho}}$ when averaged over spheres of comoving radius $R$ at time $t$. The typical overdense of region of size $R$ has $\delta^{(R)}\sim\sigma(R,t)$, and the typical underdense region has $\delta^{(R)}\sim-\sigma(R,t)$.
![[Pasted image 20251123130632.png]]
We can derive $\sigma(M,t)$ where $M=\frac{4}{3}\pi \bar{\rho}_{m_{0}}R^3$ is the average mass of matter in a sphere of comoving radius $R$. 

Linear theory: Overdense regions of radius $R$ collapse when $\delta^{(R)}\simeq 1$ which implies objects of mass $M$ typically collapse at time $t$ such that $\sigma(M,t)\simeq 1$.

Suppose $P(k)=Ak^{n}$. Simple window functions have the sane shape regardless of $R$, $W_{k}(k;R)=W_{k}(kR)$. Using the integral for $\sigma(R)$ in terms of $P(k)$ and $W_{k}(k;R)$ one gets
$$\sigma(R)\propto R^{-(n+3)/2}.\tag{21.19} $$
As $R\propto M^{1/3}$, the RMS $\sigma(M)$ for a power-law power spectra is
$$\sigma(M)\propto M^{-(n+3)/6}.\tag{21.20} $$
