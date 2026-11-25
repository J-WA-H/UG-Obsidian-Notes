The uncertainty principle is given by
$$\langle \Delta \hat{A}^2 \rangle\langle \Delta \hat{B}^2 \rangle \geq \frac{1}{4}|\langle [\hat{A},\hat{B}] \rangle |^2\tag{15.1}  .
$$It is possible for $\langle \Delta \hat{A}^2 \rangle$ to be very small if $\langle \Delta \hat{B}^2 \rangle$ is compensatingly large.

For a [[Coherent States]] and quadrature operators
$$\bra{\alpha} \hat{X}_{1}\ket{\alpha} =\frac{{\alpha+\alpha ^{*}}}{2},\;\bra{\alpha} \hat{X}_{1}^2\ket{\alpha} = {\frac{(\alpha+\alpha ^{*})^2+1}{4}}\tag{15.2}. $$Hence, $\langle \Delta X_{1}^2 \rangle=\frac{1}{4}$ and $\langle \hat{X}_{2}^2 \rangle=\frac{1}{4}$. The two quadrature uncertainties are exactly equal. Given $[\hat{X}_{1},\hat{X}_{2}]=\frac{i}{2}$ gives 
$$\frac{1}{4}|\langle [\hat{X}_{1},\hat{X}_{2}] \rangle |^2=\frac{1}{16}=\langle \Delta \hat{X}_{1}^2 \rangle \langle \Delta \hat{X}_{2} \rangle \tag{15.3} $$
so $\ket{\alpha}$ is a minimum uncertainty state.

In normal ordered form,
$$\langle \Delta \hat{X}_{1} \rangle =\frac{1}{4}\langle [(\hat{a}-\langle \hat{a} \rangle )^2+(\hat{a}^{\dagger}-\langle \hat{a}^{\dagger} \rangle )^2+2(\hat{a}^{\dagger}\hat{a}-\langle \hat{a}^{\dagger} \rangle \langle \hat{a} \rangle +1)] \rangle .\tag{15.4} $$
We can relate normally-ordered expectation values to the p-representation moments,
$$\langle \Delta \hat{X}_{1}^2 \rangle =\frac{1}{4}+\frac{1}{4}\int d^2\alpha \;p(\alpha,\alpha ^{*})[(\alpha-\langle \hat{a} \rangle )+(\alpha ^{*}-\langle \hat{a}^{\dagger} \rangle )]^2\tag{15.5}.$$
If $\langle \hat{X}_{1}^2 \rangle< \frac{1}{4}$ the integral must be negative.

The quadratic term is positive, hence the p-representation must be negative. This is not compatible with classical probability density functions.

The generalised quadrature operators are
$$\hat{X}_{1}(\vartheta)=\frac{{\hat{a}e^{ -i\vartheta/2 }+\hat{a}^{\dagger}e^{ i\vartheta/2 }}}{2},\;\hat{X}_{2}(\vartheta)=\frac{i(\hat{a}^{\dagger}e^{ i\vartheta/2 }-\hat{a}e^{ -i\vartheta/2 })}{2}.\tag{15.6} $$
Note that $\hat{X}_{1}(\pi)=\hat{X}_{1}(0)$. Equivalently,
$$\begin{bmatrix}
\hat{X}_{1}(\vartheta) \\
\hat{X}_{2}(\vartheta)
\end{bmatrix}=\begin{bmatrix}
\cos\left( \frac{\vartheta}{2} \right) & \sin\left( \frac{\vartheta}{2} \right) \\
-\sin\left( \frac{\vartheta}{2} \right) & \cos\left( \frac{\vartheta}{2} \right)
\end{bmatrix}\begin{bmatrix}
\hat{X}_{1} \\
\hat{X}_{2}
\end{bmatrix}.\tag{15.7} $$
The quadrature axes rotated by $\frac{\vartheta}{2}$ anticlockwise relative to their default positions in phase space.

Introduce the unitary squeeze operator,
$$\hat{S}(\xi)=e^{ (\xi ^{*}\hat{a}^2-\xi \hat{a}^{\dagger{2}}) /2}\tag{15.8} $$where $\hat{S}^{\dagger}(\xi)=\hat{S}(-\xi)$ and $\xi=re^{ i\theta }$, with $r$ is the squeeze parameter.

An axis $\frac{\theta}{2}$ anticlockwise from the $X_{1}$ axis defines the direction in phase space along which squeezing takes place.
![[Pasted image 20251115113837.png]]
Creation and annihilation operators transform under squeeze operators as
$$\begin{matrix}
\hat{S}^{\dagger}(\xi)\hat{a}\hat{S}(\xi)=\hat{a}\cosh(r)-\hat{a}^{\dagger}e^{ i\theta }\sinh(r) \\
\hat{S}^{\dagger}(\xi)\hat{a}^{\dagger}\hat{S}(\xi)=\hat{a}^{\dagger}\cosh(r)-\hat{a}e^{ -i\theta }\sinh(r)
\end{matrix}\tag{15.9} .$$
Set $\ket{\psi_{s}}=\hat{S}(\xi)\ket{\psi}$. Determine new quadrature uncertainties by transforming operators and taking expectation values with $\ket{\psi}$,
$$\bra{\psi_{s}} \hat{X}_{1}^2\ket{\psi_{s}}-\bra{\psi_{s}}\hat{X}_{1}\ket{\psi_{s}} ^2=\bra{\psi} [\hat{S}^{\dagger}(\xi)\hat{X}_{1}\hat{S}(\xi)]^2\ket{\psi} -\bra{\psi}\hat{S}^{\dagger}(\xi)\hat{X}_{1}\hat{S}(\xi)\ket{\psi} ^2. \tag{15.10}     $$
The general quadrature transformation is
$$\hat{S}^{\dagger}(\xi)\hat{X}_{1}\hat{S}(\xi)=\frac{1}{2}[e^{ -i\vartheta/2 }[\hat{a}\cosh(r)-\hat{a}^{\dagger}e^{i\theta  }\sinh(r)]+e^{ i\vartheta/2 }[\hat{a}^{\dagger}\cosh(r)-\hat{a}e^{ -i\theta  }\sinh(r)]].\tag{15.11} $$
Consider the squeezed vacuum $\ket{\xi}=\hat{S}(\xi)\ket{0}$. Hence $\bra{0}\hat{S}^{\dagger}(\xi)\hat{X}_{1}\hat{S}(\xi)\ket{0}=0$. Quadrature uncertainty follows entirely from $\hat{a}\hat{a}^{\dagger}=\hat{a}^{\dagger}\hat{a}+1$ terms within
$$\bra{0} [\hat{S}^{\dagger}(\xi)\hat{X}_{1}(\vartheta)\hat{S}(\xi)]^2\ket{0} .\tag{15.12} $$
Hence,
$$\langle \Delta \hat{X}_{1}(\vartheta)^2 \rangle =\frac{1}{4}[\cosh^2(r)+\sinh^2(r)-2\sinh(r)\cosh(r)\cos(\theta-\vartheta)].\tag{15.13} $$
If $\theta=\vartheta$, the $X_{1}$ axis is aligned with the axis along which squeezing occurs, and
$$\langle \Delta \hat{X}_{1}(\vartheta)^2 \rangle=\frac{e^{ -2r }}{4},\; \langle \Delta \hat{X}_{2}(\vartheta) ^2\rangle =\frac{e^{ 2r }}{4}\therefore\langle \Delta \hat{X}_{1}(\vartheta)^2 \rangle \langle \Delta \hat{X}_{2}(\vartheta)^2 \rangle=\frac{1}{16}\tag{15.14}  $$so this is a minimum uncertainty state.

Recall the unitary displacement operator $\hat{D}(\alpha)=e^{ \alpha ^{*}\hat{a}-\alpha \hat{a}^{\dagger} }$ and set
$$\ket{\alpha,\xi}=\hat{D}(\alpha)\hat{S}(\xi)\ket{0}.\tag{15.15}$$
We can similarly transform $\hat{D}^{\dagger}(\alpha)\hat{S}^{\dagger}(\xi)\hat{X}_{1}(\vartheta)\hat{S}(\xi)\hat{D}(\alpha)$ and consider the expectation values with respect to $\ket{0}$.
Set $\alpha=|\alpha|e^{ i\phi }$. It can be shown that $$\langle \Delta \hat{X}_{1}(\vartheta)^2 \rangle =\frac{1}{4}\left( \cosh^2(r)\left[ 1+2|\alpha|^2\cos^2\left( \frac{\vartheta}{2}-\phi \right) \right]+\sinh^2(r)\left[ 1+2|\alpha|^2\cos^2\left( \theta-\frac{\vartheta}{2}-\phi \right) \right]-\sinh(r)\cosh(r)((1+2|\alpha|^2)2\cos(\theta-\vartheta)\right.$$$$\left. \left .+2|\alpha|^2\left[ \cos^2\left( \frac{\theta}{2}-\phi \right)-1 \right]\right)\right).\tag{15.16} $$If $\theta=\vartheta$ and $\phi=\frac{\vartheta}{2}$, we again produce a minimum uncertainty state.

From $\hat{a}\ket{0}=0$, it follows that $\hat{S}(\xi)\hat{a}\hat{S}^{\dagger}(\xi)\hat{S}(\xi)\ket{0}=0$, and therefore
$$[\hat{a}\cosh(r)+\hat{a}^{\dagger}e^{ i\theta }\sinh(r)]\ket{\xi} =0.\tag{15.17} $$
Hence, $\ket{\xi}$ is an eigenstate of $\hat{a}\cosh(r)+\hat{a}^{\dagger}e^{ i\theta }\sinh(r)$ with eigenvalue 0.

Similarly, we note
$$\hat{D}(\alpha)\hat{S}(\xi)\hat{a}\hat{S}^{\dagger}(\xi)\hat{D}^{\dagger}(\alpha)\hat{D}(\alpha)\hat{S}(\xi)\ket{0} =0,\tag{15.18} $$therefore
$$[(\hat{a}-\alpha)\cosh(r)+(\hat{a}^{\dagger}-\alpha ^{*})e^{ i\theta }\sinh(r)]\ket{\alpha,\xi} =0\tag{15.19} .$$Hence, $\ket{\alpha,\xi}$ is an eigenstate of $\hat{a}\cosh(r)+\hat{a}^{\dagger}e^{ i\theta }\sinh(r)$ with eigenvalue $\alpha \cosh(r)+\alpha ^{*}e^{ i\theta }\sinh(r)$.