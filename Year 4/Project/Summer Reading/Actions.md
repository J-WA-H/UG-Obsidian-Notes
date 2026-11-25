To reduce the complexity of these field models, it is appropriate to integrate out these massive modes to obtain a smaller number of collective degrees of freedom.
The approximate action for a relativistic magnetic flux line is proportional to the area of the worldsheet swept out by its motion. The heuristic justification for this is quite general. In a Lorentz-invariant theory the string is invariant with respect to longitudinal Lorentz boosts; hence, one has to consider only transverse motions of the vortex. A transverse velocity $v_{\perp}$ results in a Lorentz contraction of the vortex thickness and thus, by the Lorentz invariance of $\mathcal{L}$, the vortex action must take the form
$$S=\int d^4x\mathcal{L}\propto \int dtd\ell(1-v_{\perp}^2)^{1/2}\tag{15.1} $$where $d\ell$ is the length element along the string.

The action for the [[Abelian Higgs Model]] in a general spacetime is
$$S=\int d^4y\sqrt{ -g }\left[ |\mathcal{D}_{\mu}\phi|^2-\frac{1}{4}F_{\mu \nu}F^{\mu \nu}-V(\phi) \right].\tag{15.2} $$
To obtain an effective string action, we need to find an approximate solution for a moving and curved string and then integrate out the massive transverse degrees of freedom. A Lorentz-boosted version of the static cylindrically-symmetric solutions, $(10.11-12)$, provides an appropriate starting point if the string curvature is small relative to the string width. The approximate solution is then constructed around each point $x^{\mu}(\zeta^{a})$ on a curved worldsheet swept out by the zeros of the Higgs field. The worldsheet coordinate $\zeta^{0}$ is chosen to be time-like, with the other, $\zeta^{1}$, space-like. 
Now at each point on the worldsheet we can choose two space-like vectors $n_{\mu}^{A},A=1,2$, which are normal to the tangent vectors $x^{\mu}_{a}$, that is $n^{A}_{\mu}x^{\mu}_{a}=0$. We also require these vectors to be orthonormal, $g^{\mu \nu}n_{\mu}^{A}n_{\nu}^{B}=-\delta^{AB}$. With this choice, we can reparametrise any point $y^{\mu}$ near the worldsheet using two additional radial coordinates $\rho^{A}$,
$$y^{\mu}(\xi)=x^{\mu}(\zeta)+\rho^An^{\mu}_{A}(\zeta),\tag{15.3} $$
where $\xi^{\mu}=(\zeta^{a},\rho^{A})$. The new coordinates $\xi^{\mu}$ will be single-valued if the point $y^{\mu}$ is closer to the string than its curvature $R$.
![[Pasted image 20250826153251.png]]

The approximate ansatz for the field configuration near the worldsheet is then
$$\begin{matrix}
\phi(y(\xi))=\phi_{s}(r) \\
A^{\mu}(y(\xi))-n^{\mu}_{B}(\zeta)A_{s,B}(r),
\end{matrix}\tag{15.4} $$
where the solution $(\phi_{s},A_{s})$ is given in $(10.11-12)$ and $r^2=(\rho^{1})^2+{(\rho^{2})}^2$. To change coordinates from $y^{\mu}$ to $\xi^{\mu}$ in the action $(15.2)$ we must calculate the Jacobian
$$\sqrt{ -g }\det\left( \frac{\partial y}{\partial \xi} \right)=(-\det M_{\alpha\beta})^{1/2},\tag{15.5} $$where
$$M_{\alpha\beta}=\left( g_{\mu \nu} \frac{\partial y^{\mu}}{\partial \xi^{\alpha}} \frac{\partial y^{\nu}}{\partial \xi^{\beta}} \right)=\mathrm{diag}(\gamma_{ab},-\delta_{AB})+\mathcal{O}\left( \frac{r}{R} \right)\tag{15.6} .$$
Here $\gamma_{ab}=g_{\mu \nu}x^{\mu}_{a}x^{\nu}_{b}$ is the worldsheet metric and so, defining $\gamma=\det \gamma^{ab}$, we clearly must have $\det M_{\alpha\beta}\approx \gamma$. Similarly, for the other terms in $(15.2)$, we must have $|\mathcal{D}\phi|^2\approx |\mathcal{D}_{s}\phi_{s}|^2$ and $F^{2}\approx F^2_{s}$ to an accuracy $\mathcal{O}(r/R)$. Integration over the two normal coordinates $\rho^{A}$ then yields the string energy per unit length $\mu$. Because of the rapid exponential fall-off in the string profile, the apparent inaccuracies of order $r/R$ are cut off at the string width $\delta$ and are reduced to order $\delta/R$; these are two widely disparate scales, especially in a late cosmological context. To lowest order, then, the effective string action becomes
$$S=-\mu \int d^2\zeta \sqrt{ -\gamma }.\tag{15.7} $$This is the Nambu action. This is proportional to the surface area swept out by the string in spacetime. The strings equation of motion can by obtained by varying the action with respect to $x^{\mu}(\zeta^{a})$. Using the relation
$$d\gamma=\gamma \gamma^{ab}d\gamma_{ab},\tag{15.8} $$
and the expression for $\gamma_{ab}$ we find that
$$x^{\mu;a}_{a}+\Gamma^{\mu}_{\nu\sigma}\gamma^{ab}x^{\nu}_{a}x^{\sigma}_{b}=0,\tag{15.9} $$
where $\Gamma^{\mu}_{\nu\sigma}=\frac{1}{2}g^{\mu \tau}(g_{\tau \nu,\sigma}+g_{\tau\sigma,\nu}-g_{\nu\sigma ,\tau})$ is the 4D Christoffel symbol. From the two dimensional point of view, $x^{\mu}(\zeta^{a})$ is a set of four scalar fields and the covariant Laplacian $(15.9)$ is given by
$$x^{\mu;a}_{,a}=\frac{1}{\sqrt{ -\gamma }}\partial_{a}(\sqrt{ -\gamma }\gamma^{ab}x^{\mu}_{b}).\tag{15.10} $$
The string energy-momentum tensor can be found by varying the action with respect to the metric $g_{\mu \nu}$,
$$T^{\mu \nu}\sqrt{ -g }=-2 \frac{\delta s}{\delta g_{\mu \nu}}=\mu \int d^2\zeta \sqrt{ -\gamma }\gamma^{ab}x^{\mu}_{,a}x^{\nu}_{,b}\delta^{(4)}(x^{\sigma}-x^{\sigma}(\zeta^{a})).\tag{15.11} $$

Analytical treatment of these global $U(1)$-string is difficult due to its topological coupling to the Goldstone boson field, that is, the requirement that the phase $\vartheta$ changes by $2\pi$ as the string is encircled. The fact that the energy in this massless scalar field is considerably larger than that in the string makes understanding of the string dynamics difficult. This peculiar coupling can be clarified by going over to an equivalent antisymmetric tensor representation in which the Kalb-Ramond action describes a global $U(1)$ string.

The equivalence of a real massless scalar field and a two-index antisymmetric tensor $B^{\mu \nu}$ can be readily seen by considering the relation
$$\eta \partial_{\mu}\vartheta=\frac{1}{2}\epsilon_{\mu \nu\lambda \rho}\partial^{\nu}B^{\lambda \rho}. \tag{15.12} $$
The massless wave equation $\partial_{\mu}\partial^{\mu}\vartheta=0$ is then trivially satisfied. On the other hand, a similar identity for $\vartheta$, $\epsilon^{\mu \nu\lambda \rho}\partial_{\lambda}\partial_{\rho}\vartheta=0$, implies the dual equation of motion for $B^{\mu \nu}$,
$$\partial_{\mu}H^{\mu \nu\lambda}=0,\tag{15.13} $$
where $H^{\mu \nu\lambda}$ is the field strength tensor
$$H^{\mu \nu\lambda}=\partial^{\mu}B^{\nu\lambda}+\partial^{\lambda}B^{\mu \nu}+\partial^{\nu}B^{\lambda \mu}.\tag{15.14} $$
The action for the antisymmetric field is
$$S_{H}=\frac{1}{6}\int H^2d^4x.\tag{15.15} $$
The coefficients in $(15.8)$ have been chosen so that the energy-momentum tensors for the two dual fields coincide,
$$T^{\nu}_{\;\mu}=H_{\mu\alpha\beta}H^{\nu\alpha\beta}-\frac{1}{6}\delta^{\nu}_{\;\mu}H_{\alpha\beta \gamma}H^{\alpha\beta\gamma}=2\eta^2\left( \partial_{\mu}\vartheta \partial^{\nu}\vartheta-\frac{1}{2}\delta^{\nu}_{\;\mu}\partial_{\alpha}\vartheta \partial^{\alpha}\vartheta \right),\tag{15.16}$$where the action for the massless scalar field is
$$S_{\vartheta}=\eta^2\int d^4x(\partial_{\mu}\vartheta)^2.\tag{15.17} $$
Note that the action in $(15.11)$ cannot be directly obtained by a direct substitution of $(15.8)$ into $(15.13)$ because the relation $(15.8)$ only holds if the field equations for $\vartheta$ and $B_{\mu \nu}$ are satisfied - $(15.8)$ doesn't admit arbitrary variations. However, the transition from $(15.11)$ to $(15.13)$ can be accomplished with a canonical transformation of the field variables. 
The periodic nature of $\vartheta$ and the presence of the massive field $|\phi|$ complicates the relationship between $\vartheta$ and $B^{\mu \nu}$ in the Goldstone model,
$$S=\int d^4x[(\partial_{\mu}|\phi|)^2+|\phi|^2(\partial_{\mu}\vartheta)^2-V(\phi)].\tag{15.18} $$
The Euler-Lagrange equation for $\vartheta$ is then
$$\partial_{\mu}(|\phi|^2\partial^{\mu}\vartheta)=0,\tag{15.19} $$
suggests that in this model the relation $(15.8)$ should be replaced by
$$|\phi|^2\partial_{\mu}\vartheta=\frac{1}{2}\eta\epsilon_{\mu \nu\lambda \rho}\partial^{\nu}B^{\lambda \rho}.\tag{15.20} $$
It is verified that the action $(15.14)$ is equivalent to 
$$S=\int d^4x\left[ (\partial_{\mu}|\phi|)^2+\frac{\eta^2}{6|\phi|^2}H^2-V(\phi) \right].\tag{15.21} $$
This equivalence breaks down in the presence of vortices. The field equations for $H^{\mu \nu\sigma}$ that follows from $(15.16)$ is
$$\partial_{\sigma}\left( \frac{\eta^2}{|\phi|^2}H^{\mu \nu\sigma} \right)=-\eta\epsilon^{\mu \nu\sigma \tau}\partial_{\sigma}\partial_{\tau}\vartheta\equiv{4}\pi j^{\mu \nu},\tag{15.22} $$
while the field equation obtained from the action $(15.15)$ is equal to zero, in the presence of a vortex, $\vartheta$ is a multivalued function of the coordinates and $j^{\mu \nu}\neq 0$ on the vortex core. Integrating over a two-surface orthogonal to the string yields the winding number of $\vartheta$,
$$\int_{S}d^2x\epsilon^{\mu \nu}\partial_{\mu}\partial_{\nu}\vartheta=\int_{\partial S}d\vartheta=2\pi. \tag{15.23} $$
Hence for a string lying along the $z$-axis,
$$j^{03}=\frac{\eta}{2}\delta(x)\delta(y).\tag{15.24} $$
More generally, the commutator $\epsilon^{\mu \nu\sigma \tau}\partial_{\sigma}\partial_{\tau}\vartheta$ performs a projection onto the worldsheet swept out by the line of Higgs zeros in the core of the string. If the worldsheet is parametrised as $x^{\mu}(\zeta^{a})$ then we can write
$$j^{\mu \nu}=\frac{\eta}{2}\int\delta^{(4)}[x-x(\zeta^{a})]d\sigma^{\mu \nu},\tag{15.25} $$
where
$$d\sigma^{\mu \nu}=\epsilon^{ab}x^{\mu}_{a}x^{\nu}_{b}d^2\zeta,\tag{15.26} $$is the worldsheet area element.
The source term on the right hand side of $(15.18)$ can be accounted for in the action $(15.17)$ by adding
$$4\pi \int B_{\mu \nu}j^{\mu \nu}d^4x=2\pi \eta \int B_{\mu \nu}d\sigma^{\mu \nu}.\tag{15.27} $$
The complete effective action for a global string in the antisymmetric tensor representation is then
$$S=-\mu_{0}\int \sqrt{ -\gamma }d^2\zeta+\frac{1}{6}\int H^2d^4x+2\pi \eta \int B_{\mu \nu}d\sigma^{\mu \nu}.\tag{15.28} $$
This string tension $\mu_{0}$ is found by integrating over the massive $|\phi|$ modes in $(15.17)$ for a static string solution. The first tern is the Nambu action. The second term is to compensate the singularity at the vortex core when $|\phi|=0$ by the behaviour of $H^{\mu \nu\sigma}$. The last term is the interaction of the string with the antisymmetric field $B_{\mu \nu}$, replacing the earlier topological coupling of the Goldstone boson. This string coupling to $B_{\mu \nu}$ is local and linear and resembles the pointlike interaction of the electron. Exploiting this analogy with electromagnetism makes strings become analytically more accessible.