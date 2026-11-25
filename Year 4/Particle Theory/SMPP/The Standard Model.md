The standard model is defined by the gauge group
$$SU(3)_{c}\times SU(2)_{L}\times U(1)_{Y}\tag{4.1} $$
where $SU(3)_{c}$ is the colour group, $SU(2)_{L}$ is the left handed weak isospin group and $U(1)_{Y}$ is the hypercharge group.

$SU(3)_{c}$ has 8 [generators](Non-Abelian%20Group%20Theory.md), so 8 gauge bosons, $G_{\mu}^{\;a}$ with $a=1,2,\dots,8$. The generators are defined by the Gell-Mann matrices,
$$T_{a}=\frac{g_{s}}{2}\lambda_{a}\tag{4.2} $$
with the Gell-Mann matrices normalised to $\mathrm{Tr}(\lambda_{a}\lambda_{b})=2\delta_{ab}$. Gell-Mann matrices are 3x3 traceless Hermitian matrices

$SU(2)_{L}$ has 3 generators so 3 gauge bosons, $W_{\mu}^{\;I}$ with $I=1,2,3$. The generators are defined by the Pauli matrices
$$T_{I}=\frac{g}{2}\sigma_{I}\tag{4.3}$$
which are normalised to $\mathrm{Tr}(\sigma^a\sigma^b)=2\delta^{ab}$.

$U(1)_{Y}$ has 1 generator so 1 gauge boson $B_{\mu}$. The generators are defined by
$$Q_{Y}g'\mathbb{I}\tag{4.4} $$
where $Q_{Y}$ is the hypercharge, $g'$ is the coupling constant and $\mathbb{I}$ is the identity.

The field strength for the gluon field is
$$G_{\mu \nu}=\partial_{\mu}G_{\nu}^{\;a}-\partial_{\nu}G_{\mu}^{\;a}-\frac{ig_{s}}{2}[G_{\mu}^{\;a}\lambda_{a},G_{\nu}^{\;a}\lambda_{a}]\tag{4.5}. $$
We can also define the covariant gauge derivative
$$\mathcal{D}_{\mu}\equiv \partial_{\mu}+i \frac{g_{s}}{2}G_{\mu}^{\;a}\lambda^a+i \frac{g}{2}W_{\mu}^{\;I}\sigma^I+ig'Q_{Y}B_{\mu}\tag{4.6}. $$
To define chirality, we use the $\gamma$-matrices, $\{ \gamma^\mu,\gamma^\nu \}=2\eta^{\mu \nu}$. We can define
$$\gamma^5\equiv i\gamma^{0}\gamma^{1}\gamma^{2}\gamma^{3}\tag{4.7} .$$
This can be used to define left and right handed projection operators,
$$P_{L}=\frac{{1-\gamma_{5}}}{2};\; P_{R}=\frac{{1+\gamma_{5}}}{2}\tag{4.8}. $$
These projection operators obey
$$\begin{matrix}
P_{L}+P_{R}=1 \\
P_{L,R}^2=P_{L,R} \\
P_{L}P_{R}=0
\end{matrix}.\tag{4.9} $$
The left handed fermion field is defined as $\psi_{L}\equiv P_{L}\psi$ and the right handed fermion field is given by $\psi_{R}\equiv P_{R}\psi$, where $\psi$ is the Dirac field. $\psi_{L},\psi_{R}$ are irreducible representations of the Lorentz to group. $SU(2)_{L}$ only acts on $\psi_{L}$.

The fields we have are the left handed quark doublet
$$q_{L}=\begin{bmatrix}
u_{L} \\
d_{L}
\end{bmatrix}\tag{4.10}. $$
$u_R,d_{R}$ exist but not in a doublet. We also have the left handed lepton doublet
$$\ell_{R}=\begin{bmatrix}
\nu_{L} \\
e_{L}
\end{bmatrix}\tag{4.11} $$
where $e_{R}$ does exist but $\nu_{R}$ does not.

|             | $q_{L}$       | $u_{R}$       | $d_{R}$        | $\ell_{L}$     | $e_{R}$ | $H$           |
| ----------- | ------------- | ------------- | -------------- | -------------- | ------- | ------------- |
| $SU(3)_{c}$ | $\mathbf{3}$  | $\mathbf{3}$  | $\mathbf{3}$   | $-$            | $-$     | $-$           |
| $SU(2)_{L}$ | $\mathbf{2}$  | $-$           | $-$            | $\mathbf{2}$   | $-$     | $\mathbf{2}$  |
| $U(1)_{Y}$  | $\frac{1}{6}$ | $\frac{2}{3}$ | $-\frac{1}{3}$ | $-\frac{1}{2}$ | $-1$    | $\frac{1}{2}$ |

We can now form the Standard Model Lagrangian. First write the Lagrangian that takes into account the interaction between the gauge fields and matter interacts,
$$\mathcal{L}_{gauge}=-\frac{1}{8}\mathrm{Tr}[G_{\mu \nu}G^{\mu \nu}]-\frac{1}{8}\mathrm{Tr}[W_{\mu \nu}W^{\mu \nu}]-\frac{1}{9}B_{\mu \nu}B^{\mu \nu}+\sum_{\psi_{L}}i\bar{\psi}_{L}\gamma_{\mu}\mathcal{D}_{L}^{\;\mu}\psi_{L}+\sum_{\psi_{R}}i\bar{\psi}_{R}\gamma_{\mu}\mathcal{D}^{\mu}_{R}\psi_{R}+\mathcal{D}^\mu H^{\dagger}\mathcal{D}_{\mu}H\tag{4.12} $$
where $\psi_{L}$ sums over $q_{L},\ell_{L}$ and $\psi_{R}$ sums over $u_{R},d_{R},e_{R}$.
This assumes all particles are massless, which is not the case, which is solved by the Higgs mechanism, given by the Yukawa Lagrangian
$$\mathcal{L}_{Yukawa}=-Y_{u}\bar{q}_{L}\tilde{H}u_{R}-Y_{d}\bar{q}_{L}Hd_{R}-Y_{\ell}\bar{\ell}_{L}He_{R}+\mathrm{H.c.}\tag{4.13} $$
and the potential
$$V_{H}=-m_{H}^2H^{\dagger}H+\lambda(H^{\dagger}H)^2\tag{4.14} $$
where $\tilde{H}$ is $\tilde{H}=i\sigma_{z}H^{*}$.

This gives the Standard Model Lagrangian,
$$\mathcal{L}_{SM}=-\frac{1}{8}\mathrm{Tr}[G_{\mu \nu}G^{\mu \nu}]-\frac{1}{8}\mathrm{Tr}[W_{\mu \nu}W^{\mu \nu}]-\frac{1}{9}B_{\mu \nu}B^{\mu \nu}+\sum_{\psi_{L}}i\bar{\psi}_{L}\gamma_{\mu}\mathcal{D}_{L}^{\;\mu}\psi_{L}+\sum_{\psi_{R}}i\bar{\psi}_{R}\gamma_{\mu}\mathcal{D}^{\mu}_{R}\psi_{R}+\mathcal{D}^\mu H^{\dagger}\mathcal{D}_{\mu}H$$
$$-Y_{u}\bar{q}_{L}\tilde{H}u_{R}-Y_{d}\bar{q}_{L}Hd_{R}-Y_{\ell}\bar{\ell}_{L}He_{R}+\mathrm{H.c.}+m_{H}^2H^{\dagger}H-\lambda(H^{\dagger}H)^2\tag{4.15} .$$
This has parameters $g_{s},g,g',Y_{u},Y_{d},Y_{\ell},m_{H},\lambda$.

This is just for the first generation, so we can add a generation index to account for the whole standard model, but the overall structure remains the same.

A renormalisable theory means we must have a mass dimension $\leq 4$, which comes from the action $S=\int d^4x \mathcal{L}$.
$$\begin{matrix}
\mathrm{dim}(\psi)=\frac{3}{2} \\
\mathrm{dim}(H)=1 \\
\mathrm{dim}(\mathcal{D}_{\mu})=1
\end{matrix}\tag{4.16}. $$
The Standard Model is a gauge theory but it has some global symmetries:
- Baryon number $Q_{B}(q_{L},u_{R},d_{R})=\frac{1}{3}(q_{L},u_{R},d_{R})$ $Q_{B}(\bar{q}_{L},\bar{u}_{R},\bar{d}_{R})=-\frac{1}{3}(\bar{q}_{L},\bar{u}_{R},\bar{d}_{R})$.
- Lepton number $L_{e},L_{\mu},L_{\tau}$. $L_{e}e=+1 e$.

Lepton number is nor mixed by $SU(3)_{c}$.