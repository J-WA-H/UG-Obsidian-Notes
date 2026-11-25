 There are two main steps to calculate the $2\to 2$ scattering amplitude in the $\frac{\lambda \phi^4}{4!}$ theory.
1. Consider $G_{4}(x_{1},x_{2},x_{3},x_{4})=\bra{0}T\left( \hat{\phi}(x_{1})\hat{\phi}(x_{2})\hat{\phi}(x_{3})\hat{\phi}(x_{4})e^{ -i \int d^4y\,\mathcal{H}_{int}(\hat{\phi}(y)) } \right)\ket{0}$.
2. Use the LSZ reduction formula to compute the $S$-matrix which gives the scattering amplitude.

Consider step 1: From [[Wick's Theorem]] and [[Feynman Rules]],
$$G_{4}(x_{1},x_{2},x_{3},x_{4})^{\mathcal{O}(\lambda^{1})}_{connected}=-i\lambda \int d^4y\,G_{F}(x_{1}-y)G_{F}(x_{2}-y)G_{F}(x_{3}-y)G_{F}(x_{4}-y)\tag{11.1} $$
with
$$G_{F}(x-y)=\int \frac{d^4y}{(2\pi)^4}e^{ -ip_{\mu}(x-y)^{\mu} } \frac{-i}{p_{\mu}p^{\mu}-m^2+i\varepsilon}.\tag{11.2} $$
$G_4$ can be represented as
![[Pasted image 20251111160938.png]]
where the centre point, $y$ is represented by the factor $V_{4}\int d^4y$, with the n-point vertex defined as
$$V_{n}=\left.\frac{\partial^n\mathcal{L}_{int}}{\partial \phi^n} \right|_{\phi=0}.\tag{11.3} $$
For $n=4$,
$$\mathcal{L}_{int}=-\mathcal{H}_{int}=-\frac{i\lambda}{4!}\phi^4\implies V_{4}=\frac{\partial^4\mathcal{L}_{int}}{\partial \phi^4}=-i\lambda.\tag{11.4} $$
From Feynman rules, the lines connecting $x_{i}$ to $y$ is represented by the [[Feynman Propagator]] $G_{F}(x_{i}-y)$. We also need to divide by a symmetry factor.

Now consider step 2: Fourier transform $G_{4}(x_{1},x_{2},x_{3},x_{4})\to \tilde{G}_{4}(p_{1},p_{2},p_{3},p_{4})$, where $+p_{i}$ represents incoming momentum and $-p_{j}$ represents outgoing momentum.
$$\tilde{G}_{4}(p_{1},p_{2},p_{3},p_{4})=\prod_{i=1}^{4}\int \frac{d^4x_{i}}{(2\pi)^4}e^{ +i\sum_{i=1}^{4}p_{i}^{\mu}x_{i\mu} }G_{4}(x_{1},x_{2},x_{3},x_{4}).\tag{11.5} $$
Evaluating this gives
$$\tilde{G}_{4}(p_{1},p_{2},p_{3},p_{4})=-i\lambda(2\pi^4)\delta^{(4)}(p_{1}+p_{2}+p_{3}+p_{4})\prod_{j=1}^{4} \frac{i}{p^2_{j}-m^2+i\varepsilon}\tag{11.6}. $$The inclusion of the $\delta$-function makes sure momentum is conserved.
![[Pasted image 20251111162326.png]]
Reading from this gives the Feynman rules in momentum space:
1. Each internal line with momentum $p^{\mu}$ is represented by the propagator
$$\frac{i}{p^2-m^2+i\varepsilon}\tag{11.7} $$
2. Each vertex contributes a factor of $-i\lambda$
3. For each external line write down $e^{ -ipx }$ where all external momenta $p^{\mu}$ are counted as incoming
4. Impose momentum conservation at each vertex
5. Integrate over each undetermined (loop) momentum
$$\int \frac{d^4p}{(2\pi)^4}$$
6. Divide by the symmetry factor.

Now the Greens function has been determined we can apply LSZ reduction to $\tilde{G}_{4}$.

In position space, LSZ reduction is given by $$i\prod_{i=1}^{4}(\square_{x_{i}}+m^2)G_{4}\tag{11.8} $$so in momentum space it is given by
$$\left. i\prod_{i=1}^{4} (p_{i}^2-m^2) \right|_{p_{0i}=E_{pi}=+\sqrt{ |\vec{p}_{i}|^2_{m^2} }}.\tag{11.9} $$
This gives for $2\to 2$ scattering, the S-matrix is given by
$$S_{p_{1},p_{2}\to k_{1},k_{2}}\equiv (2\pi)^4\delta^{(4)}(p_{1}+p_{2}-k_{1}-k_{2})\mathcal{M}_{p_{1}p_{2}\to k_{1}k_{2}}.\tag{11.10} $$
From the $\delta$-function, $S$ is not finite so the finite scattering amplitude is given by $\mathcal{M}$. To compute $\mathcal{M}$, we need very similar Feynman rules, only considering internal lines
![[Pasted image 20251111163658.png]]
Every internal line gives a factor $-i\lambda$ and every external line gives a factor of $1$.

For some general theory, 
$$\mathcal{L}_{gen}=\hat{\phi}\circ \hat{\mathbb{K}}\circ \hat{\phi}+\mathcal{L}_{int}(\hat{\phi}),\tag{11.11} $$
$$G_{F}(p)=-i \hat{\mathbb{K}}^{-1}.\tag{11.12} $$
For example, if $$\mathcal{L}_{int}=\frac{\lambda'}{3!}\phi^3+\frac{\lambda}{4!}\phi^4.\tag{11.13} $$There is a three-point vertex for the $\phi^3$ term and a 4-point vertex for $\phi^4$.
![[Pasted image 20251111164226.png]]
