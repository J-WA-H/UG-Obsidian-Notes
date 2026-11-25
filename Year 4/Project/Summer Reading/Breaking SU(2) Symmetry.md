An example of $SU(2)$ gauge invariance is isospin where a two component nucleon spinor transforms as
$$\begin{bmatrix}
\psi_{p} \\
\psi_{n}
\end{bmatrix}\to \begin{bmatrix}
\psi'_{p} \\
\psi'_{n}
\end{bmatrix}=U\begin{bmatrix}
\psi_{p} \\
\psi_{n}
\end{bmatrix}\tag{3.1} $$
where $U\in SU(2)$ and can be written in the general form
$$U=\exp(i\theta \hat{n}_{a} \tau_{a})=\cos\left( \frac{\theta}{2} \right)+2i\hat{n}_{a}\tau_{a}\sin\left( \frac{\theta}{2} \right)\tag{3.2} $$
where $\tau_{a}=\sigma_{a}/2$ and $\hat{n}_{a}$ is a unit 3-vector.

$\tau^{a}$ has the same eigenvalues of $T^{a}$ so $T^2=\tau^{a}\tau^{a}$, analogous to angular momentum with eigenvalues $T(T+1)$. For $T=1$, the isospin system is in the triplet which represents $SU(2)$ as the generators are given by the structure constants $(T_{i})_{jk}=-i\epsilon_{ijk}$.
These are rotation matrices which form a representation of $SO(3)$, which obeys the same commutation relations as $SU(2)$ but globally the two groups are not identical.

The parameter manifold for $SU(2)$ is the 3-sphere $S^3$, while for $SO(3)$ it is $S^{3}$ with opposite points on the sphere identical.

The representation of $SU(2)$ is given by the dimension of $\tau^{a}$, i.e. for $T=\frac{1}{2}$, this is 2-representation as $\tau^{a}$ has dimension 2.

One example of $SU(2)$ symmetry breaking is $SU(2)\xrightarrow{2} I$. Consider that the Higgs field transforms as a two-component spinor in fundamental 2-representation of $SU(2)$,
$$\sigma=\begin{bmatrix}
\sigma_{1} \\
\sigma_{2}
\end{bmatrix} \tag{3.3} ,$$
$\sigma_{1},\sigma_{2}\in \mathbb{C}$.
This symmetry can be broken with a quartic potential $V(\sigma)$ whose zeros are fields with $\sigma ^{\dagger}\sigma=\eta^2$, which is some positive constant.
Taking $\sigma_{0}^{\dagger}=(0,\eta)$, it can be seen that $H$ is empty since no generators can annihilate $\sigma_{0}$, so $\mathcal{M}=SU(2)$. Rewriting $\sigma$ as four real fields shows that this is isomorphic to $S^3$ in four Euclidean dimensions.
Coupling $\sigma$ to the three gauge fields $W_{a}^{\mu}$ we have the transformations
$$\sigma\to U\sigma;\;\mathcal{G}_{\mu \nu}=U\mathcal{G}_{\mu \nu}U^{-1} \tag{3.4} $$
where $U\in SU(2)$ and $\mathcal{G_{\mu\nu}}=G^{\mu \nu}_{a}\tau_{a}$; $G^{\mu \nu}_{a}=\partial^{\mu}W^{\nu}_{a}-\partial^{\nu}W^{\mu}_{a}+e\epsilon_{abc}W^{\mu}_{b}W^{\nu}_{c}$.
Counting the components for this symmetry breaking we see that there are three massless Goldstone bosons absorbed, and one massive Higgs boson will remain.