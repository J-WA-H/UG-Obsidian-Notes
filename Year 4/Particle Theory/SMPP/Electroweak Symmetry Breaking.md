The electroweak group is a sub set of [[The Standard Model]], which breaks into the electromagnetic group
$$SU(2)_{L}\times U(1)_{Y}\to U(1)_{em}\tag{5.1}. $$
To define spontaneous symmetry breaking, consider the Higgs boson - a Lorentz scalar, $SU(2)$ doublet. It has a vacuum expectation value (VEV)
$$\bra{0} H\ket{0} \equiv \langle H \rangle =\begin{bmatrix}
0 \\
\frac{v}{\sqrt{ 2 }}
\end{bmatrix}\tag{5.2} $$where $v\approx 246\text{ GeV}$.

The Higgs potential is
$$V(H)=-m_{H}^2H^{\dagger}H+\lambda(H^{\dagger}H)^2,\tag{5.3} $$
![[Pasted image 20260217114932.png]]
From this the value of the VEV (minima) can be determined.
$$\frac{dV}{dH}=-m_{H}H^{\dagger}+2\lambda(H^{\dagger}H)H^{\dagger}=0\implies \langle H^{\dagger}H \rangle =\frac{m_{H}^2}{2\lambda}\tag{5.4}. $$
Substitute $\langle H \rangle$ into $\mathcal{L}_{SM}$, consider $\mathcal{D}_{\mu}H^{\dagger}\mathcal{D}^{\mu}H$:
$$\mathcal{D}_{\mu}\langle H \rangle =\frac{i}{2}\begin{bmatrix}
g'B_{\mu}+gW_{\mu}^{3} & g(W_{\mu}^{1}-iW_{\mu}^2) \\
g(W_{\mu}^1+iW_{\mu}^2) & g'B_{\mu}-gW_{\mu}^3
\end{bmatrix}\begin{bmatrix}
0 \\
\frac{v}{\sqrt{ 2 }}
\end{bmatrix}\tag{5.5} =\frac{iv}{2\sqrt{ 2 }}\begin{bmatrix}
g(W_{\mu}^1-iW_{\mu}^2) \\
g'B_{\mu}-gW_{\mu}^3
\end{bmatrix}.$$
This gives
$$\mathcal{D}_{\mu}\langle H^{\dagger} \rangle \mathcal{D}^{\mu}\langle H \rangle =\frac{v^2}{2}\left( \frac{g^2}{4}\underbrace{ (W_{\mu}^1-iW_{\mu}^2U) }_{ \sqrt{ 2 }W_{\mu}^+ }\underbrace{ (W_{\mu}^1+iW_{\mu}^2) }_{ \sqrt{ 2 }W_{\mu}^- }+\underbrace{ \left( \frac{g'}{2}B_{\mu}-\frac{g}{2}W_{\mu}^3 \right)^2 }_{ \frac{g^2}{4\cos^2\theta_{w}}Z_{\mu}Z^\mu } \right)\tag{5.6} $$where the weak angle $\theta_{w}$ is defined such that $\tan \theta_{w}=\frac{g'}{g}$. This gives
$$\mathcal{D}_{\mu}\langle H^{\dagger} \rangle \mathcal{D}^{\mu}\langle H \rangle=\frac{v^2}{2}\left( \frac{g^2}{2}W_{\mu}^{+}W^{-\mu }+\frac{g^2}{4\cos^2\theta_{w}}Z^\mu Z_{\mu} \right)$$
This then gives masses to the weak gauge bosons,
$$M_{W}=\frac{gv}{2};\;M_{Z}=\frac{gv}{2\cos \theta_{w}}\tag{5.7}. $$
The non-zero VEV of the Higgs field gives the weak bosons its mass. The photon $A_{\mu}$ remains massless.
$$\begin{bmatrix}
Z_{\mu} \\
A_{\mu}
\end{bmatrix}=\begin{bmatrix}
\cos \theta_{w} & -\sin \theta_{w} \\
\sin \theta_{w} & \cos \theta_{w}
\end{bmatrix}\begin{bmatrix}
W_{\mu}^3 \\
B_{\mu}
\end{bmatrix}\tag{5.8} $$
where $W_{\mu}^3,B_{\mu}$ are the original massless fields.

We can then get a modified covariant derivative,
$$\mathcal{D}_{\mu}=\partial_{\mu}+\frac{ig}{\sqrt{ 2 }}(\sigma^+W_{\mu}^++\sigma^-W_{\mu}^-)+\frac{ig}{2}\sigma^3(c_{w}Z_{\mu}+s_{w}A_{\mu})+ig'Q_{Y}(-s_{w}Z_{\mu}+c_{w}A_{\mu})\tag{5.9} $$
where
$$\sigma^+=\frac{{\sigma^1+i\sigma^2}}{\sqrt{ 2 }};\;\sigma^{-}= \frac{{\sigma^1-i\sigma^2}}{\sqrt{ 2 }}\tag{5.10} $$
and $c_{w}\equiv \cos \theta_{w}$, $s_{w}\equiv \sin \theta_{w}$. The $Z_{\mu},A_{\mu}$ terms then simplify to 
$$i\left( \frac{g}{2}\sigma^3c_{w}-g'Q_{Y}s_{w} \right)Z_{\mu}+i\left( \frac{g}{2}\sigma^3s_{w}+g'Q_{Y}c_{w} \right)A_{\mu}=\frac{ig}{c_{w}}\left( \frac{\sigma^3}{2}c_{w}^2-Q_{Y}s_{w}^2 \right)Z_{\mu}+igs_{w}\left( \frac{\sigma^3}{2}+Q_{Y} \right)A_{\mu}\tag{5.11}. $$
From this the gauge coupling is $e=gs_{w}$, and $\frac{\sigma^3}{2}+Q_{Y}$ is the unbroken generator.

For $\psi_{L}$: $Q_{em}= \frac{\sigma_{3}}{2}+Q_{Y}^L$; $\psi_{R}$: $Q_{Y}^R\implies \left( \frac{\sigma^3}{2}+Q_{Y}^L \right)P_{L}+Q_{Y}^{R}P_{R}$.

|          | $q_{L}=(u_{L},d_{L})$                     | $\ell_{L}=(\nu_{L},R_{L})$ | $U_{R}$       | $d_{R}$        | $e_{R}$ |
| -------- | ----------------------------------------- | -------------------------- | ------------- | -------------- | ------- |
| $Q_{Y}$  | $\frac{1}{6}$                             | $-\frac{1}{2}$             | $\frac{2}{3}$ | $-\frac{1}{3}$ | $-1$    |
| $Q_{em}$ | $\left( \frac{2}{3},-\frac{1}{3} \right)$ | $(0,-1)$                   | $\frac{2}{3}$ | $-\frac{1}{3}$ | $-1$    |
This shows $Q_{em}$ is not chiral since $R$ and $L$ handed particles have the same change.

The weak field strength tensor can be written as
$$W_{\mu \nu}=\partial_{\mu}W_{\nu}^I\sigma^I-\partial_{\nu}W_{\mu}^I\sigma^I+\frac{ig}{2}[W_{\mu}^I\sigma^I,W_{\nu}^J\sigma^J]=\partial_{\mu}W_{\nu}^I\sigma^I-\partial_{\nu}W_{\mu}^I\sigma^I-\frac{ig}{2}W_{\mu}^IW_{\nu}^J(2i\varepsilon_{ijk}\sigma_{k})\tag{5.12} .$$
Using $W_{\mu}^{\pm}=\frac{1}{\sqrt{ 2 }}(W_{\mu}^1\mp iW_{\mu}^2)$, we get
$$W_{\mu \nu}^{\pm}=(\partial_{\mu}\mp igW_{\mu}^{3})W_{\nu}^{+}-(\partial_{\nu}\mp igW_{\nu}^{3})W_{\mu}^{\pm}\tag{5.13} $$
From this, we get the [non-abelian nature](Yang-Mills%20Theory.md) of the electroweak bosons
![[Pasted image 20260217161502.png]]
Consider the Yukawa Lagrangian
$$\mathcal{L}_{Y}=-\bar{q}_{L}Y_{u}\langle \tilde{H} \rangle u_{R}-\bar{q}_{L}Y_{d}\langle H \rangle d_{R}-\bar{\ell}_{L}Y_{\ell}\langle H \rangle e_{R}+\text{H.c.}=-\bar{u}_{L}Y_{u} \frac{v}{\sqrt{ 2 }}u_{R}-\bar{d}_{L}Y_{d} \frac{v}{\sqrt{ 2 }}d_{R}-\bar{e}_{L}Y_{e} \frac{v}{\sqrt{ 2 }}e_{R}+\text{H.c}\tag{5.14} .$$
The Higgs VEV gives the fermion masses, and leaves neutrinos massless.

The massless Dirac equation is
$$i\gamma^{\mu}\partial_{\mu}\psi =0\tag{5.15} .$$
In the Weyl basis,
$$\gamma^{0}=\begin{bmatrix}
0 & \mathbb{I}_{2\times 2} \\
\mathbb{I}_{2\times 2} & 0
\end{bmatrix};\;\gamma^{i}=\begin{bmatrix}
0 & \sigma^i \\
-\sigma^i & 0
\end{bmatrix}\tag{5.16} .$$
This gives
$$i\gamma^{0}\partial_{0}\begin{bmatrix}
\psi_{L} \\
\psi_{R}
\end{bmatrix}=\begin{bmatrix}
i\partial_{0}\psi_{R} \\
i\partial_{0}\psi_{L}
\end{bmatrix};\;i\gamma^{i}\partial_{i}\begin{bmatrix}
\psi_{L} \\
\psi_{R}
\end{bmatrix}=\begin{bmatrix}
0 & \sigma^{i}\partial_{i} \\
-\sigma^{i}\partial_{i} & 0
\end{bmatrix}\begin{bmatrix}
\psi_L \\
\psi_{R}
\end{bmatrix}\tag{5.17} .$$
This gives
$$(i\partial_{t}-i\vec{\sigma}\cdot \vec{\nabla})\psi_{L}=m\psi_{R},\;(i\partial_{t}+i\vec{\sigma}\cdot\vec{\nabla})\psi_{R}=m\psi_{L}\tag{5.18}. $$
The spin operator is $S=\frac{\sigma}{2}$, which can then be used to define helicity, the spin projection onto the 3-momentum,
$$h=\frac{{\vec{s}\cdot \vec{p}}}{|\vec{p}|}\tag{5.19} $$
![[Pasted image 20260217163054.png]]
Right handed particles have helicity $h_{R}=\frac{1}{2}$ and left handed particles have helicity $h_{L}=-\frac{1}{2}$. For example, $W^{+}$ has a spin +1 in the $z$-direction. $W^+\to e^{+}\nu$. In the centre of mass frame
![[Pasted image 20260217163245.png]]
For the first case, the neutrino helicity $h_{\nu}=\frac{1}{2}$ implies they are right-handed, but as right-handed neutrinos don't exist we can't use this. Therefore, the bottom scenario is the only valid one.

For electroweak coupling,
$$\mathcal{D}_{\mu}=\partial_{\mu}+Z_{\mu} \frac{ig}{c_{w}}\left[ \left( \frac{\sigma_{3}}{2}-Q_{Y}^Ls_{w}^2 \right)P_{L}-Q_Y^Rs_{w}^2P_{R} \right]+\frac{ig}{\sqrt{ 2 }}\begin{bmatrix}
0 & W_{\mu}^+ \\
W_{\mu}^- & 0
\end{bmatrix}P_{L}+ieQ_{em}A_{\mu}\tag{5.20}$$
We can rewrite the square bracket as
$$Q_{em}=\left( \frac{\sigma_{3}}{2}+Q_{Y}^L \right)P_{L}+Q_{Y}^RP_{R}\tag{5.21} $$
$$\implies \mathcal{D}_{\mu}=\partial_{\mu}+Z_{\mu} \frac{ig}{c_{w}}\left[ \left( \frac{\sigma_{3}}{2}-Q_{em}s_{w}^2 \right)P_{L}-Q_{em}s_{w}^2P_{R} \right]+\dots=+\dots\left[ \frac{\sigma_{3}}{2}P_{L}-Q_{em}s_{w}^2 \right]\tag{5.22}. $$
In the final expression, the $\sigma_{3}P_{L}$ part is the chiral part and the $Q_{em}s_{w}^2$ is the vector part.

