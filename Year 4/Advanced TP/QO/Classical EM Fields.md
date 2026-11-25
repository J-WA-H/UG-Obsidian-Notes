In SI units, Maxwell's equations are
$$\begin{matrix}
\vec{\nabla}\times \vec{E}=-\frac{{\partial \vec{B}}}{\partial t} & \vec{\nabla}\times \vec{B}=\mu_{0}\varepsilon_{0} \frac{{\partial \vec{E}}}{\partial t} \\
\vec{\nabla}\cdot \vec{E}=0 & \vec{\nabla}\cdot \vec{B}=0.
\end{matrix}\tag{2.1} $$
Electromagnetic fields are considered to generate from scalar and vector potentials,
$$\vec{E}=-\vec{\nabla}\Phi-\frac{\partial \vec{B}}{\partial t}\;\;\vec{B}=\vec{\nabla}\times \vec{A}.\tag{2.2} $$
Gauge freedom is the choice of potentials without changing the physical fields.

The Coulomb/radiation gauge is $\vec{\nabla}\cdot \vec{A}=0$ and far from charges $\Phi=0$. This gives the fields
$$\vec{E}=-\frac{\partial \vec{A}}{\partial t}\;\;\vec{B}=\vec{\nabla}\times \vec{A}.\tag{2.3} $$
Using Maxwell's equations this gives
$$\nabla ^2\vec{A}-\frac{1}{c^2} \frac{{\partial^2\vec{A}}}{\partial t^2}=0.\tag{2.4} $$
The periodic boundary conditions are equivalent to propagation around a ring cavity of path $L$. The solution to this is given by sines and cosines represented by $\exp\left( \pm \frac{i\pi x}{L} \right)/\sqrt{ L }$.
![[Pasted image 20251010105325.png]]
The $\pm$ in the exponential implies different directions - $+$ for clockwise propagation and $-$ for anticlockwise propagation.

This is only for 1 dimension, while for realistic scenarios you need three dimensions in a large volume $V$.
$$\vec{A}(\vec{r},t)=\sum_{\vec{k},s}\vec{e}_{\vec{k},s}[A_{\vec{k},s}(t)e^{ i\vec{k}\cdot \vec{r} }+\text{c.c.}]\tag{2.5} $$where $\text{c.c.}$ is the complex conjugate. In a cubical cavity $V=L^3$ and $\vec{k}=\frac{2\pi}{L}\begin{bmatrix}m_{x} \\ m_{y} \\ m_{z}\end{bmatrix}$. The sum is over $\vec{k}$ and the two polarisation directions.
From the gauge condition $\vec{\nabla}\cdot \vec{A}=0$, $\vec{\nabla}\cdot(\vec{e}_{\vec{k},s}e^{ i\vec{k}\cdot \vec{r} })=0$ hence $\vec{e}_{\vec{k},s}\cdot \vec{k}=0$ so the polarisation is orthogonal to the direction of propagation.
The vectors $\vec{e}_{\vec{k}{1}}$ and $\vec{e}_{\vec{k}2}$ form a right handed orthogonal basis. The wave equation for $\vec{A}(\vec{r},t)$ now yields
$$\frac{d^2{A}_{\vec{k}s}}{dt^2}=-\omega^2_{k}A_{{\vec{k}s}}(t)\tag{2.6} $$
where $\omega_{k}=ck$ and $k=|\vec{k}|$.
This is a harmonic oscillator with solution
$$A_{\vec{k}s}(t)=A_{\vec{k}s}(0)e^{ -i\omega_{k}t }.\tag{2.7} $$
This gives the EM fields
$$\vec{E}(\vec{r},t)=i\sum_{\vec{k},s}\omega_{\vec{k}}\vec{e}_{\vec{k},s}[A_{\vec{k},s}(t)e^{ i\vec{k}\cdot \vec{r} }-\text{c.c.}],\tag{2.8} $$
$$\vec{B}(\vec{r},t)=\frac{i}{c}\sum_{\vec{k},s}\omega_{\vec{k}}(\vec{k}\times\vec{e}_{\vec{k}s})[A_{\vec{k},s}(t)e^{ i\vec{k}\cdot \vec{r} }-\text{c.c.}].\tag{2.9} $$
The electromagnetic field energy $H$ is
$$H=\frac{1}{2}\int d^3r\left( \varepsilon_{0}\vec{E}\cdot \vec{E}+\frac{1}{\mu_{0}}\vec{B}\cdot \vec{B} \right).\tag{2.10} $$
This is integrating the electromagnetic energy density over the volume $V$.
This then reveals the interacting Hamiltonian
$$H=2\varepsilon_{0}V\sum_{\vec{k},s}\omega_{\vec{k}}A^{*}_{\vec{k},s}A_{\vec{k},s}.\tag{2.11} $$
