By the [fundamental theorem](Homotopy%20Groups.md), $(9.3)$, strings can arise at a symmetry breaking $G\to H$ for which the unbroken subgroup $H$ is disconnected. For a non-abelian group $G$, a variety of broken generators can usually be employed to pass between the disconnected components of $H$, $T^{S}$ which corresponds to the minimum energy string configuration. At large distances from an axisymmetric string, as we wind around by an angle $\theta$, the Higgs field at $\theta=0$ will rotate as
$$\tag{11.1} \phi(\theta)=U(\theta)\phi(0)=\exp(iT^{S}\theta)\phi(0).$$
Because $G$ is non-abelian, this rotation will generally affect the embedding of $H$ in $G$, yielding a continuous family of different, but isomorphic, subgroups $H(\theta)$. In the general case, then, the generators of the algebra rotate non-trivially and the local unbroken symmetry group $H$ cannot be globally extended. The subgroup of globally well-defined symmetries, known as the centraliser $\hat{H}$, is defined as
$$\tag{11.2} \hat{H}=\{ h\in H\;|\;[U(2\pi),D(h)]=0 \},$$
where $D$ is the appropriate Higgs representation of $G$ and $H=H(0)$.

$(11.1)$ is only valid in one particular gauge. To find a more general form of $\phi(\theta)$, we note that outside the string core the gauge-covariant derivative $\phi$ vanishes,
$$\tag{11.3} \mathcal{D}_{\mu}\phi=(\partial_{\mu}-ieA^{a}_{\mu}T^{a})\phi=0.$$
It follows that $U(\theta)$ is given by the path-ordered exponential,
$$U(\theta)=P\exp\left( ie\int_{0}^{\theta}dx^{\mu}A^{a}_{\mu}T^{a} \right).\tag{11.4} $$
A complete winding about a string must yield $U(2\pi)=D(h)$m where $h\in H$ lies in a component of $H$ not connected to the identity. In the gauge $(11.1)$, $A^{a}_{\mu}T^{a}=A^{S}_{\mu}T^{S}$, path-ordering is unnecessary and we can write $U(2\pi)=\exp(ieT^{S}\Phi^{S})$ where $\Phi^{S}$ is the non-abelian magnetic flux associated with $A^{S}_{\mu}$. Since $U(2\pi)$ is non-trivial, it is clear that $\Phi^{S}\neq 0$.
The Higgs field for the axisymmetric string solution $\phi(r,\theta)=U(\theta)\phi(r,0)$ does not have to vanish at $r=0$. For regularity at the origin, we only have to require that $U(\theta)$ leaves $\phi(0,0)$ invariant, $U(\theta)\phi(0,0)=\phi(0,0)$. Hence, a more general ansatz for a global non-abelian string can be written as
$$\phi(r,\theta)=U(\theta)[f(r)\phi(\infty,0)+\sigma(r)], \tag{11.5} $$where $f(r)\to 1$ and $|\sigma(r)|\to 0$ as $r\to \infty$. Now consider the transformations of the form
$$\tag{11.6} h(\theta)=g(\theta)h(\theta)g^{-1}(\theta),$$
where $U(\theta)=D(g(\theta))$ and $h\in H$. This leaves the solution $\phi(\infty,0)$ at spatial infinity invariant, since $D(h)\phi(\infty,0)=\phi(\infty,0)$, but it may affect the $\sigma$-fields in the string interior. If $D(h)\sigma(r)=0\;\forall\;r$, then the transformation acts trivially. However, it is possible for $D(h)$ to act non-trivially on $\sigma$, if the string generator remains invariant, $hL^{S}h^{-1}=L^{S}$, that is, $h\in H$. In this case, the energies of this inequivalent configurations is the same, which gives the existence of the a zero mode.
The transformation $(11.6)$ can be promoted become spacetime dependent, $h(z,t)$ which corresponds to massless excitations which propagate along the string at the speed of light.

The simplest way to form non-abelian strings is through the maximal breakdown of an $SU(N)$ symmetry, $SU(N)\to \mathbb{Z}_{N}$, achieved by taking $N$ Higgs fields in the adjoint representation and choosing an appropriate potential. The $\mathbb{Z}_{2}$-string is the most cosmologically interesting. The Lagrangian for this Higgs model is
$$\mathcal{L}=\frac{1}{2}\mathcal{D}_{\mu}\vec{\varphi} \mathcal{D}^{\mu}\vec{\varphi}+\frac{1}{2}\mathcal{D}_{\mu}\vec{\psi} \mathcal{D}^{\mu}\vec{\psi}-\frac{1}{4}\mathrm{Tr}(\mathcal{G}_{\mu \nu}\mathcal{G}^{\mu \nu})-V(\vec{\varphi},\vec{\psi}),\tag{11.7} $$
where $\varphi,\psi$ transforms in the adjoint representation of $SU(2)$ and, with generators $T^a$ and [gauge fields](Breaking%20SU(2)%20Symmetry.md) $W^{a}_{\mu}$. The potential is of the form
$$\tag{11.8} V(\vec{\varphi},\vec{\psi})=\frac{1}{4}\lambda_{\phi}(\varphi^2-\eta^2_{\phi})^2+\frac{1}{4}\lambda_{\psi}(\psi^2-\eta_{\psi}^2)^2+\frac{1}{8}g(\vec{\varphi} \cdot \vec{\psi})^2.$$
The field equations are then
$$\tag{11.9} \begin{matrix}
\mathcal{D}_{\mu}\mathcal{D}^{\mu}\vec{\varphi}=\frac{\partial V}{\partial \varphi}, & \mathcal{D}_{\mu}\mathcal{D}^{\mu}\vec{\psi}=\frac{\partial V}{\partial \psi}, \\
\mathcal{D}_{\mu}G^{\mu \nu}_{a}=j^{\nu}_{a},
\end{matrix}$$
where
$$\tag{11.10} j^{\nu}_{a}=e\epsilon_{abc}((\mathcal{D}^{\nu}\varphi)_{b}\vec{\phi}_{c}+(\mathcal{D}^{\nu}\psi)_{b}\vec{\psi}_{v}).$$
We look for cylindrically symmetric vortex solutions similar to the [[Abelian Higgs Model]] with the ansatz
$$\tag{11.11} \begin{matrix}
\vec{\varphi}=\eta_{\phi}\hat{z} \\
\vec{\psi}=\eta_{\psi}f(r)(\cos \theta,\sin \theta,0) \\
\vec{W}_{\theta}=-\frac{1}{e}\alpha(r)\hat{z}.
\end{matrix}$$
The minimum energy configuration with $\varphi$ remaining in the vacuum state depends on the condition $\lambda_{\phi}\eta_{\phi}^{4}>\lambda_{\psi}\eta_{\psi}^4$, otherwise $\varphi$ and $\psi$ would exchange roles. $f(r),\alpha(r)$ has the same boundary conditions between as the abelian Higgs model, and substituting these in gives identical to $(10.14-15)$ for the $n=1$ vortex.
The magnetic field decays exponentially from a maximum at the core on a characteristic length-scale $(e\eta_{\psi})^{-1}$, while the Higgs field $\psi$ rises from zero to its vacuum expectation value $\eta_{\psi}$ on a length scale $(\sqrt{ \lambda_{\psi}\eta_{\psi} })^{-1}$.
The magnetic flux of the vortex solution can be defined by the field tensor
$$\tag{11.12} F^{\mu \nu}=\frac{1}{\eta_{\phi}}\phi_{a}G^{\mu \nu}_{a}.$$
With $\vec{\varphi}$ lying along the z-axis, $B_{z}=G_{12}^{3}$ so from Stokes' theorem, the magnetic flux of the $\mathbb{Z}_{2}$ string is
$$\Phi_{B}=\frac{2\pi}{e}\tag{11.13}. $$
These strings have an interesting internal structure as they appear at a second-stage symmetry breaking after the monopoles have emerged. The monopole flux is confined and so the monopole becomes attached to two $\mathbb{Z}_{2}$ strings, each taking away half of the original magnetic flux. Strings and antistrings are not identical and segments of string with opposite flux are separated by these beadlike solitons. Note that many winding number configurations are possible. A single bead passing along the string will change the winding by 2, hence strings with odd windings $n=\pm 1,\pm 3,\dots$ belong to the same topologically non-trivial sector, while even windings are topologically equivalent to the vacuum.

The [SO(10)](GUT.md) symmetry breaking scheme provides a useful example of a realistic grand unified model with strings. These strings are associated with an unbroken discrete $\mathbb{Z}_{2}$ symmetry, with some significant differences to $\mathbb{Z}_{2}$ strings. For these phenomenological strings, they are associated with an $SO(10)$ operator which rotates the identity from the non-trivial element of $\mathbb{Z}_{2}$. The string will have a radius of $\delta \sim(e \eta)^{-1}$ and energy $\mu\sim \eta^2$ where $\eta\sim 10^{16}\text{ GeV}$ corresponds to the $\mathbf{126}$ Higgs symmetry breaking scale. Subsequent symmetry breaking at the electroweak phase transition employs a Higgs field in the $\mathbf{10}$-representation with components in $(8.7)$. None of these have eigenvalue $P=0$ so they introduce an unacceptable phase factor on passing around a string. To avoid this, we must rotate to an alternative operator $R$ also generating a non-trivial element of $\mathbb{Z}_{2}$, but such that $R\phi_{10}=0$. This means at the electroweak scale, some additional flux will be squeezed into the string core. The layered internal structure of these $SO(10)$ strings depend on the symmetry breaking scheme, and other GUT strings can be expected to have different internal structures. Strings do not appear in the electroweak symmetry breaking in the standard model.

Alice strings arise from the symmetry breaking $SO(3)\xrightarrow{\mathbf{5}}O(2)$. This symmetry leaves an unbroken $SO(2)$ component which contains rotations about the $z$-axis. There is also a disconnected component which is generated from the first by a $180^{\circ}$ rotation about an axis lying in the $xy$-plane. In the presence of a string, the symmetric tensor field rotates as
$$\Phi(\theta)=\exp(\theta T_{1}/2)\Phi(0)\exp(-\theta T_{1}/2). \tag{11.14} $$
This results in a corresponding rotation of the unbroken $SO(2)$ within $SO(3)$ with $\Phi\equiv Q$ and $Q(0)=T^{3}$. This charge operator $Q$ is double-valued, since $Q(2\pi)=-Q(0)$, which creates difficulties in interpreting the electrodynamics of this model. Defined relative to $Q(\theta)$, the electromagnetic gauge potential $A^{q}_{\mu}=\cos\left( \frac{\theta}{2} \right)W^{3}_{\mu}+\sin\left( \frac{\theta}{2} \right)W^{2}_{\mu}$ is likewise double-valued, as the electric and magnetic fields are given by
$$F_{\mu \nu}=\cos\left( \frac{\theta}{2} \right)G^{3}_{\mu \nu}+\sin\left( \frac{\theta}{2} \right)G^2_{\mu \nu}\tag{11.15}. $$
To study Maxwell's equations, we introduce a branch cut from the string centre at $x=0$ to $x=\infty$, along which we impose the boundary condition that $F^{above}_{\mu \nu}=-F^{below}_{\mu \nu}$. This apparent change in the sign of the electromagnetic field is unobservable because the charge $Q$ of a test particle transported across the cut will also change sign to $-Q$. As a result there is no discontinuous change in the force on the particle.
The presence of an Alice string affects a nearby charged particle. Consider a particle on the negative $x$-axis, near a string lying along the $z$-axis. By reflection symmetry it is clear that $E_{x},E_{z}$ must be equal above and below the cut. From the boundary condition $\vec{E}^{above}=-\vec{E}^{below}$ it gives that only $E_{y}$ is non-zero. This is also the boundary condition for a conducting plate, so we can expect the particle to experience a force from its image charge and, thus, to be attracted towards the string. It will only be possible to globally define the charge within a Gaussian surface which encloses two strings since a finite branch cut can pass between them, as shown below
![[Pasted image 20250811210535.png]]
If a charged particle were to travel between two strings, its charge would change from $Q$ to $-Q$ while the strings would acquire a charge $2Q$. This is manifested as a non-local Cheshire charge which emanates from the branch cut between the strings, with the branch cut now acting as if there were a charged conducting plate. Magnetic monopoles in the model cause similar effects, however we do not expect Alice strings in our universe because charge conjugation is not an observed symmetry.

Semilocal strings occur in models possessing both local and global symmetries. A simple model is given by the Lagrangian
$$\mathcal{L}=|(\partial_{\mu}-ieA_{\mu})\Phi|^2-\frac{1}{4}F_{\mu \nu}F^{\mu \nu}-\frac{1}{4}\lambda(\Phi ^{\dagger}\Phi-\eta^2)^2\tag{11.16} $$
where $\Phi=\begin{bmatrix}\phi,\chi\end{bmatrix}$ is a complex scalar doublet. This model is invariant under global $SU(2)_{g}$ transformations, $\Phi \to \exp (i\omega^{a}\tau^{a})$ and under local $U(1)_{l}$ transformations, $\Phi\to \exp[i\alpha(x)\mathbb{I}]\Phi$. When $\Phi$ acquires a vacuum expectation value, the symmetry is broken to a global $U(1)$,
$$SU(2)_{g}\times U(1)_{l}\to U(1)_{g}. \tag{11.17} $$
In the basis where $\Phi=(\phi,0)$, the unbroken $U(1)_{g}$ is the group of global phase rotations of $\chi$. The vacuum manifold of $\Phi$ is a three-sphere, $\Phi ^{\dagger}\Phi=\eta^2$. Since the [homotopy group](Homotopy%20Groups.md) is $\pi_{1}(S^{3})=\mathbb{I}$, all loops in $\mathcal{M}$ can be contracted to a point, and the model has no topological strings. However, when global symmetries are present, one should consider the gradient energy cost associated with the variation of $\Phi$ along a loop. Only for special loops which are generated by acting with elements of $U(1)_{l}$ on some $\Phi\in \mathcal{M}$ can the scalar gradient energy be compensated by the gauge field. A string configuration in which $\Phi$ traverses one of these loops on a path around the string can be stabilised by the gradient energy barrier that must be overcome if the loop is to be contracted to a point.
The existence of string solutions with this Lagrangian is easily verified if we set $\Phi=(\phi,0)$, which reduces $(11.16)$ to the [[Abelian Higgs Model]] with solutions
$$\begin{matrix}
\Phi=(\phi_{s},0) & A^{\mu}=A^{\mu}_{s}
\end{matrix}\tag{11.18} $$
where $\phi_{s},A^{\mu}_{s}$ are the same as in $(10.11-12)$. Equivalent solutions can be obtained by acting these solutions with global rotations and gauge transformations. 
An important difference between semilocal strings and topological strings is that the vanishing of $\Phi$ on the string axis is not enforced for topological reasons. One can construct field configurations which never leave the vacuum manifold and have the same asymptotic behaviour as the solutions in $(11.18)$. For example, we have
$$\begin{matrix}
\Phi=(f(r)e^{ i\theta },g(r)) & A_{\theta}=v(r)/er
			\end{matrix}\tag{11.19} $$where $f(r)=r(a^2+r^2)^{-1/2}$, $g(r)=a(a^2+r^2)^{-1/2}$, $v(r)=r^2(a^2+r^2)^{-1}$ and $a$ is a constant parameter. The stability of the string solution depends on whether or not its energy is smaller than that of configurations like $(11.19)$. For semilocal string, $\beta<1$ produce stable strings while $\beta<1$ are unstable with respect to the formation of a scalar condensate with subsequent growth of the condensate radius $a$.

Consider the $SU(2)\times U(1)$ model. If the $SU(2)$ symmetry is gauged, it becomes identical to the Higgs sector of the standard electroweak model. The corresponding Lagrangian can be written as
$$\tag{11.20} \mathcal{L}=|\mathcal{D}_{\mu}\Phi|^{2}-\frac{1}{4}F_{B}^2-\frac{1}{4}F_{W}^{2}-\frac{1}{4}\lambda(\Phi ^{\dagger}\Phi-\eta^2)^2$$where
$$\mathcal{D}_{\mu}=\left( \partial_{\mu}-ig\tau^{a}W_{\mu}^{a}-\frac{i}{2}g'B_{\mu} \right)\Phi \tag{11.21} $$
and the factor $\frac{1}{2}$ has been introduced in order to confirm with the standard notation. This model has the vortex solutions
$$\begin{matrix}
\Phi=(0,\phi_{s}) & Z_{\mu}=A_{s\mu} & A_{\mu}=W_{\mu}^{1}=W_{\mu}^2=0
\end{matrix}\tag{11.22} $$
where
$$Z_{\mu}=W^{3}_{\mu}\cos \theta-B_{\mu}\sin \theta,\;A_{\mu}=W^{3}_{\mu}\sin \theta+B_{\mu}\cos \theta \tag{11.23} $$
and $\tan \theta=\frac{g'}{g}$.

The semilocal string solution is recovered from the limit $g\to 0$. Since the semilocal strings are stable for $\beta<1$, we expect electroweak strings to be stable when $g=0$ and $0<\beta<1$. However, these strings are unstable for realistic parameter values in the electroweak model although there are extensions to the standard model for which the string solutions are stable. Electroweak strings can never be absolutely stable because, unlike semilocal strings, they are separated from the vacuum by only a finite gradient energy barrier. These strings can decay quantum mechanically by the nucleation of monopole-antimonopole pairs. For $g\ll g'$, the tunnelling action is proportional to $g^{-2}$ and becomes infinite in the semilocal limit $g\to 0$.