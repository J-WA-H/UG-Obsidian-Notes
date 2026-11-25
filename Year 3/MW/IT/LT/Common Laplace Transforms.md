There are many common [[Laplace Transform]] that frequently come up.
$$\mathcal{L}[1](s)=\frac{1}{s}$$
$$\mathcal{L}[t^n](s)=\frac{n!}{s^{n+1}}$$
for $n\in \mathbb{N}$. For non-integer $n$ this is generalised to the gamma function
$$\mathcal{L}[t^n](s)=\frac{\Gamma(n+1)}{s^{n+1}}$$
where $$\Gamma(n)=\int_{0}^{\infty}t^{n-1}e^{-t}dt.$$
$$\mathcal{L}[e^{\lambda t}](s)=\frac{1}{s-\lambda};\;s>\mathrm{Re}[\lambda]$$
$$\mathcal{L}[\sin \omega t](s)=\frac{\omega}{s^2+\omega^2}$$
$$\mathcal{L}[\cos \omega t](s)=\frac{s}{s^2+\omega^2}$$
$$\mathcal{L}[\sinh \omega t](s)=\frac{\omega}{s^2-\omega^2}$$
$$\mathcal{L}[\cosh \omega t](s)=\frac{s}{s^2-\omega^2}$$
$$\mathcal{L}[\delta(t-t')](s)=e^{-st'}.$$
