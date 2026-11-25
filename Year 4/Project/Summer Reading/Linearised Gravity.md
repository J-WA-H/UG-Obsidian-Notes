For non-relativistic static matter, the energy-momentum tensor is
$$T^{\mu}_{\;\nu}=\mathrm{diag}(\rho,-p_{1},-p_{2},-p_{3})\tag{19.1} $$so the Newtonian limit of the Einstein equations becomes
$$\nabla^2\Phi=4\pi G(\rho+p_{1}+p_{2}+p_{3}),\tag{19.2} $$
where $\Phi$ is the gravitational potential. For non-relativistic, $p_{i}\ll \rho$ so $\nabla^2\Phi=4\pi G\rho$.

For strings, they have a large longitudinal tension. For a straight string along the $z$-axis, $p_{3}=-\rho$, while $p_{1},p_{2}$ vanish when averaged over the string cross-section. From this the right-hand side of $(19.2)$ vanishes so straight strings produce no gravitational force on surrounding matter. However, considering relativistic motion like an oscillating loop can be strong emitters of gravitational radiation. 
A gravitational string is described by the combined system of Einstein, Higgs, and gauge field equations. Although there has been no exact solutions found, in most applications there are two major simplifications. First is assuming that the string thickness is much smaller than all other relevant dimensions - the string is approximated as a one dimensional line with a delta-function distributional energy momentum tensor, [(16.12)](Strings%20in%20Flat%20Spacetime.md). Secondly, the gravitational field of the string is assumed to be sufficiently weak that the linearised Einstein equations can be employed - although this are not valid for supermassive strings.

In a weak gravitational field, the spacetime metric is almost Minkowskian,
$$\begin{matrix}
g_{\mu \nu}=\eta_{\mu \nu}+h_{\mu \nu}, & |h_{\mu \nu}|\ll 1,\tag{19.3} 
\end{matrix}$$
and the Einstein equations can be linearised in $h_{\mu \nu}$. The linearised equations take a simple form in the harmonic gauge,
$$\Box h_{\mu \nu}=-16\pi GS_{\mu \nu},\tag{19.4} $$
where
$$S_{\mu \nu}=T_{\mu \nu}-\frac{1}{2}\eta_{\mu \nu}T^{\sigma}_{\;\sigma}\tag{19.5} $$
with the energy-momentum tensor $T_{\mu \nu}$ and with indices raised and lowered using the Minkowski metric $\eta_{\mu \nu}$. The harmonic gauge is specified by the conditions
$$\partial_{\nu}\left( h^{\nu}_{\;\mu}-\frac{1}{2}\delta^{\nu}_{\;\mu}h^{\sigma}_{\;\sigma} \right)=0.\tag{19.6} $$
In the limit of zero string thickness, the string energy-momentum tensor is given by $(16.12)$
$$T^{\mu \nu}(\vec{r},t)=\mu \int d\zeta(\dot{x}^{\mu}\dot{x}^{\nu}-x'^{\mu}x'^{\nu})\delta^{(3)}(\vec{r}-\vec{x}(\zeta,t)).\tag{16.12} $$
For a straight static string lying along the $z$-axis,
$$T^{\mu}_{\;\nu}=\mu\delta(x)\delta(y)\mathrm{diag}(1,0,0,1),\tag{19.7} $$
and the solution of $(19.4)$ is
$$\begin{matrix}
h_{00}=h_{33}=0, \\
h_{11}=h_{22}=8G\mu \ln\left( \frac{r}{r_{0}} \right),
\end{matrix}\tag{19.8} $$where $r=(x^2+y^2)^{1/2}$ and $r_{0}$ is a constant of integration. At large distances from the string, $h_{\mu \nu}$ becomes large and the weak-field approximation breaks down.

Rewrite the metric from $(19.8)$ in cylindrical coordinates,
$$ds^2=dt^2-dz^2-(1-h)(dr^2+r^2d\theta^2),\tag{19.9} $$
where
$$h=8G\mu \ln\left( \frac{r}{r_{0}} \right)\tag{19.10}.$$
Introducing a new radial coordinate $r'$ as
$$(1-h)r^2=(1-8G\mu)r'^2\tag{19.11} ,$$
we obtain, to linear order in $G\mu$,
$$ds^2=dt^2-dz^2-dr'^2-(1-8G\mu)r'^2d\theta^2.\tag{19.12} $$
Finally, introduce a new angular coordinate,
$$\theta'=(1-4G\mu)\theta,\tag{19.13} $$
the metric takes a Minkowskian form,
$$ds^2=dt^2-dz^2-dr'^2-r'^2d\theta'^2.\tag{19.14} $$
This shows that the geometry around a straight cosmic string is locally identical to flat spacetime. This geometry is however not globally Euclidean, since the angle $\theta'$ varies in the range
$$0\leq \theta'<2\pi(1-4G\mu).\tag{19.15} $$Hence, the effect of the string is to introduce an azimuthal 'deficit angle',
$$\Delta=8\pi G\mu,\tag{19.16} $$implying that a surface of constant $t,z$ has the geometry of a cone rather than a plane.
The dimensionless parameter $G\mu$ plays an important role in the physics of cosmic strings. Its magnitude is given by [(7.3)](Cosmic%20Strings),
$$\tag{19.17} G\mu\sim \left( \frac{\eta}{m_{pl}} \right)^{2},$$
where $m_{pl}$ is the plank mass.'
The weak-field approximation $(19.3)$ is justified if $G\mu\ll 1$ or, equivalently, $\eta\ll m_{pl}$. The string scenario for galaxy formation requires $G\mu\sim 10^{-6}$, corresponding to a grand-unified scale $\eta\sim 10^{16}\text{ GeV}$, while observations constrain $G\mu$ to be less than $\sim 10^{-5}$.