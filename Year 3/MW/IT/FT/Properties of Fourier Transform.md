The [[Fourier Transform]] has many useful properties.
- Linearity: For any function $f(x),g(x)$ and scalars $a,b\in \mathbb{C}$:
	$$\mathcal{F}[af(x)+bg(x)](k)=a\mathcal{F}[f(x)](k)+b\mathcal{F}[g(x)](k)$$
	$$\mathcal{F}^{-1}[a\tilde{f}(k)+b\tilde{g}(k)](x)=a\mathcal{F}^{-1}[\tilde{f}(k)](x)+b\mathcal{F}^{-1}[\tilde{g}(k)](x).$$
- Translation
	$$\mathcal{F}[f(x-x_{0})](k)=e^{-ikx_{0}}\mathcal{F}[f(x)](k)$$
	$$\mathcal{F}^{-1}[\tilde{f}(k-k_{0})](x)=e^{ik_{0}x}\mathcal{F}^{-1}[\tilde{f}(k)].$$
	Proof:
	$$\mathcal{F}[f(x-x_{0})](k)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dxf(x-x_{0})e^{-ikx}$$
	Sub $x'=x-x_{0}$
	$$\mathcal{F}[f(x-x_{0})](k)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dx'f(x')e^{-ik(x'+x_{0})}$$
	$$=\frac{e^{-ikx_{0}}}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dx'f(x')e^{-ikx'}$$
	$$=e^{-ikx_{0}}\tilde{f}(k)\;\square$$
- Scaling: For $\lambda>0$
	$$\mathcal{F}[f(\lambda x)](k)=\frac{1}{\lambda}\tilde{f}\left( \frac{k}{\lambda} \right)$$
	Proof:
	$$\mathcal{F}[f(\lambda x)](k)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}f(\lambda x)e^{-ikx}dx.$$
	Sub $x'=\lambda x$
	$$\mathcal{F}[f(\lambda x)](k)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty} \frac{dx'}{\lambda}f(x')e^{-i(k/\lambda)x'}$$
	$$=\frac{1}{\lambda} \frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dx' f(x')e^{-i(k/\lambda)x'}$$
	$$=\frac{1}{\lambda}\tilde{f}\left( \frac{k}{\lambda} \right)\;\square.$$
- If $f(x):\mathbb{R}\to \mathbb{R}$, then
	$$\tilde{f}^{*}(k)=\tilde{f}(-k).$$
- If $f$ is real and even:
	 $$\tilde{f}(k)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}f(x)\cos(kx)dx.$$
- If $f$ is real and odd:
	$$\tilde{f}(k)=-\frac{i}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}f(x)\sin(kx)dx.$$
- Derivatives of a Fourier transform:
	$$\mathcal{F}[f^{(n)}(x)](k)=(ik)^{n}\tilde{f}(k).$$
	Proof:
	$$\mathcal{F}[f'(x)](k)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dx \frac{df}{dx}e^{-ikx}=\frac{1}{\sqrt{ 2\pi }}\cancelto{0}{[f(x)e^{-ikx}]_{-\infty}^{\infty}}-\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dxf(x)(-ik)e^{-ikx}$$
	$$=ik\tilde{f}(k)\;\square$$
	$$\mathcal{F}[x^nf(x)](k)=(i)^n \frac{d^n}{dx^n}\tilde{f}(k).$$
	Proof:
	$$\frac{d\tilde{f}}{dk}=\frac{1}{\sqrt{ 2\pi }} \frac{d}{dk}\int_{-\infty}^{\infty}f(x)e^{-ikx}dx=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}f(x) \frac{d}{dk}(e^{-ikx})dx$$
	$$=-\frac{i}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty} xf(x)e^{-ikx}dx=-i\mathcal{F}[xf(x)](k)\;\square$$
- Convolution: 
	$$(f*g)(x)=\int ^{\infty}_{-\infty}g(x-y)f(y)dy.$$
	Properties:
	- Commutativity: $f*g=g*f$
	- Scalars $a,b$: $f*(ag+bh)=a(f*g)+b(f*h)$
	- $\mathcal{F}[f*g](k)=\sqrt{ 2\pi }\tilde{f}(k)\tilde{g}(k)$
		Proof:
		$$\mathcal{F}[f*g](k)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dxe^{-ikx}\int_{-\infty}^{\infty}dyg(x-y)f(y)$$
		Sub $z=x-y$
		$$\mathcal{F}[f*g](k)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dyf(y)\int_{-\infty}^{\infty}dze^{-ik(y+z)}$$
		$$=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dyf(y)e^{-ikz}\int_{-\infty}^{\infty}dzg(z)e^{-ikz}\cdot \frac{\sqrt{ 2\pi }}{\sqrt{ 2\pi }}$$
		$$=\sqrt{ 2\pi }\tilde{f}(k)\tilde{g}(k)\;\square$$
