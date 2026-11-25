There are three generations in the standard model. For quarks, we have 3 up type quarks, $u^i=(u^1,u^2,u^3)=(u,c,t)$, and three down type quarks $d^i=(d^1,d^2,d^3)=(d,s,b)$.

We don't know why there are three generations.

Flavour blind interactions couple to all flavours in the same way, for example a photon with current
$$A_{\mu}\bar{d}^i\gamma^{\mu}d^{i}\tag{11.1} .$$
Most interactions are flavour blind, except for masses and Higgs couplings. These come from [Yukawa interactions](The%20Standard%20Model.md),
$$\mathcal{L}_{Y}=-\frac{v}{\sqrt{ 2 }}(\bar{q}_{L}^{i}(Y_{u})_{ij}u_{R}^{j}+\bar{q}_{L}^{i}(Y_{d})_{ij}d^j_{R}+\bar{\ell}_{L}(Y_{L})_{ij}e_{R}^{j}+\text{h.c})\tag{11.2} $$
The $Y_{i}$'s are $3\times 3$ Yukawa matrices, which in general are non-diagonal and not real.

We want to study the mass eigenbasis which diagonalises the Yukawa matrices.
$$Y_{u}=U_{L}^{u}y_{u}(U_{R}^{u})^{\dagger}\tag{11.3} $$
where $U$ is unitary. This gives
$$y_{u} \frac{v}{\sqrt{ 2 }}=\text{diag}(m_{u},m_{c},m_{t})\tag{11.4} .$$
If we rotate the fields, 
$$\begin{matrix}
u_{L}=U^u_{L}u'_{L} & \bar{u}_{L}=(U^u_{L}u'_{L})^{\dagger}\gamma^0=u_{L}'^{\dagger} \gamma^0(U_{L}^u)^{\dagger}=\bar{u}'_{L}(U_{L}^u)^{\dagger} \\
u_{R}=U^u_{R}u'_{R}
\end{matrix}\tag{11.5} .$$
Subbing this into the current gives
$$\bar{u}_{L}Y_{u}u_{R}=\bar{u}_{L}'(U_{L}^u)^{\dagger}U_{L}^uy_{u}(U_{R}^u)^{\dagger}U_{R}^uu_{R}=\bar{u}'_{L}y_{u}u_{R}\tag{11.6}. $$
We get a hierarchy of quark masses,
![[Pasted image 20260310200330.png]]
There is a strong hierarchy in quark and lepton mass. This is not explained by the standard model.

Most gauge couplings are flavour blind. For example, photon couplings
$$\bar{d}^i\gamma^\mu d^i=\bar{d}'U^{\dagger}U\gamma^{\mu}d'=\bar{d}'\gamma^{\mu}d'\tag{11.7} $$
and chiral couplings
$$\bar{\psi}\gamma_{\mu}(v+a\gamma_{5})\psi=\psi ^{\dagger}\gamma^{0}\gamma_{\mu}(v+a\gamma_{5})(P_{L}+P_{R})\psi=\psi ^{\dagger}\gamma^{0}P_{R}\gamma_{\mu}(v+a\gamma_{5})\psi_{L}+\psi ^{\dagger}\gamma^{0}P_{L}\gamma_{\mu}(v+a\gamma_{5})\psi_{R}$$
$$=\underbrace{ \psi ^{\dagger}P_{L}^{\dagger}\gamma^{0} }_{ \psi_{L} }\gamma_{\mu}(v+a\gamma_{5})\psi_{L}+\underbrace{ \psi ^{
\dagger}P_{R}^{\dagger}\gamma^{0} }_{ \psi_{R} }\gamma_{\mu}(v+a\gamma_{5})\psi_{R}\tag{11.7} .$$
This uses the relations $P_{L}\gamma_{5}=\gamma_{5}P_{L}$, $P_{R}\gamma_{\mu}=\gamma_{\mu}P_{R}$, $P_{L,R}^{\dagger}=P_{L,R}$.

This shows that the general fermions do not mix left and right chirality.

The exception is the W-boson because it mixes up/down flavours.
$$-\frac{1}{\sqrt{ 2 }}gW_{\mu}^{+}(\bar{u}_{L}\gamma^{\mu}d_{L}+\bar{\nu}_{L}\gamma^{\mu}e_{L})=-\frac{1}{\sqrt{ 2 }}gW_{\mu}^{+}(\bar{u}_{L}'\underbrace{ (U_L^{u})^{\dagger}U_{L}^d }_{ V_{CKM} }+\bar{\nu}_{L}'\underbrace{ (U_{L}^\nu)^{\dagger}U_{L}^e }_{ U_{PMNS} }e'_{L})\tag{11.8}. $$
The CKM matrix mixes quark flavour and the PMNS matrix mixes neutrino flavour. These matrices are unitary with off-diagonal elements. This allows the jumping between flavours and generations. For example, an up can change to a strange,
![[Pasted image 20260310203024.png]]
Flavour changing neural currents - these do not exist at tree level in the standard model.

Consider the meson $$D^+(c\bar{d})\to \begin{cases}
\pi^0(d\bar{d})\mu^+\nu_{\mu} \\
\pi^+(u\bar{d})\mu^+\mu^-
\end{cases}\tag{11.9} $$![[Pasted image 20260310204052.png]]
the ratio in matrix elements is
$$\frac{\mathcal{M}_{FCNC}}{\mathcal{M}_{FCCC}}\sim \frac{g^2}{(4\pi)^2} \frac{m_{d{j}}^2}{m_{W}^2}V_{uj}V_{jc}^{\dagger}\ll 1\tag{11.10} $$
For kaon decay,
![[Pasted image 20260310204314.png]]
$$\frac{\mathcal{M}_{FCNC}}{\mathcal{M}_{FCCC}}\sim \frac{g^2}{(4\pi)^2} \frac{m_{uj}^2}{m_{W}^2}V_{dj}V_{js}\ll 1\tag{11.11}. $$
We still don't know why there are 3 generations. Consider two generations, the CKM matrix is $2\times 2$.
$$V=e^{ iX}\begin{bmatrix}
e^{ i\alpha }\cos \theta & e^{ i\beta }\sin \theta \\
-e^{ i\beta }\sin \theta & e^{ -i\alpha }\cos \theta
\end{bmatrix}\tag{11.12}. $$
Rephase the quark fields,
$$u_{i}\to e^{ i\phi_{j} }u_{i},\qquad d_{j}\to e^{ i\phi_{j} }d_{j}\tag{11.13}. $$
In principle we have $4-1=3$ quarks rephasings. This gives no surviving phases in the CKM matrix.

If it was $3\times 3$, we get $6$ phases $\frac{n(n+1)}{2}$. Quark rephasing gives 5 rephasings - this gives one CP-violating phase.

CP symmetry is a discrete symmetry. C swaps particles$\leftrightarrow$antiparticles, and P swaps spatial coordinates $\vec{x}\leftrightarrow-\vec{x}\implies$ helicity flips. For CP conservation to hold, $\Gamma(A_{L}\to B_{L})=\Gamma(\bar{A}_{R}\to \bar{B}_{R})$. CP violation is shown when those two decay widths differ.

CP violation has been observed in kaon decay,
$$k_{1}=\frac{1}{\sqrt{ 2 }}(k^{0}+\bar{k}^{0}),\qquad k_{2}=\frac{1}{\sqrt{ 2 }}(k^{0}-\bar{k}^{0}),\qquad k_{2}\to 2\pi \tag{11.14}. $$
CP is violated in the flavour sector of the standard model.

