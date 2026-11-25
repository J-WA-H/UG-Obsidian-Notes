Discrete [[Fourier Transform]] gives the Fourier transform over a finite interval $[0,L]$.
$$\int_{-\infty}^{\infty}\to \int_{0}^{L}.$$
There are two cases, the first where $x$ is continuous.
In this case $f(x)$ can be expressed as a [Fourier series](Fourier%20Transform%20from%20Fourier%20Series.md) 
$$f(x)=\sum_{m=-\infty}^{\infty}c_{m}e^{ikx}$$
where
$$c_{m}=\frac{1}{\sqrt{ L }}\int_{0}^{L}f(x)e^{ikx}dx.$$
We can use this to define
$$f(x)=\frac{1}{\sqrt{ L }}\sum_{k}\tilde{f}(k)e^{ikx}$$
where $$\tilde{f}(k)=\frac{1}{\sqrt{ L }}\int_{0}^{L}dxf(x)e^{-ikx}.$$
This is valid if:
- $f$ is periodic, $f(x+L)=f(x)$
- $k$ is discrete, $k=m \frac{2\pi}{L}$, $m\in \mathbb{Z}$.

The other case is where $x$ is discrete and $x\in[0,L]\implies f$ is also discrete.
In this case $x=n\Delta x$ where $\Delta x$ are discrete intervals and $0\leq n\leq N-1$, where $n$ is the measurement number.

$f(x)$ is discretised into $f_{n}(x)$ where $f_{1}=f(x_{1}),f_{2}=f(x_{2}),\dots$.
$$\tilde{f}_{m}=\frac{1}{\sqrt{ L }}\sum_{n=0}^{N-1}f_{n}e^{-ik_{m}x_{n}}=\frac{1}{\sqrt{ L }}\sum_{n=0}^{N-1}f_{n}e^{-i_{2}\pi m/L\cdot nL/N}$$
This gives
$$\tilde{f}_{m}=\frac{1}{\sqrt{ L }}\sum_{n=0}^{N-1}f_{n}e^{-i{2}\pi mn/N}$$
$$f_{n}=\frac{1}{\sqrt{ L }}\sum_{m=0}^{N-1}\tilde{f}_{m}e^{i{2}\pi mn/N}.$$
The discrete Fourier transform can be expressed as a matrix equation:
$$\begin{bmatrix}
\tilde{f}_{0} \\
\tilde{f}_{1} \\
\vdots \\
\tilde{f}_{m}
\end{bmatrix}=\frac{1}{\sqrt{ N\Delta x }}\begin{bmatrix}
1 & 1 & \dots & 1 \\
1 & e^{-2\pi/N\;1\cdot 1} & \\
\vdots  &  & \ddots & \\
1 &  &  & e^{-i{2}\pi/N\;n\cdot m}
\end{bmatrix}\begin{bmatrix}
f_{0} \\
f_{1} \\
\vdots \\
f_{n}
\end{bmatrix}.$$
This is an $n\times m$ matrix.
