In [flat spacetime](Strings%20in%20Flat%20Spacetime.md), [(15.8)](Actions.md) becomes
$$\ddot{x}^{\mu}-x''^{\mu}+\Gamma^{\mu}_{\nu\sigma}(\dot{x}^{\nu}\dot{x}^{\sigma}-x'^{\nu}x'^{\sigma})=0.\tag{17.1} $$
Applying the conformal gauge $(16.4)$ allowed $\zeta^{0}=x^{0}$. However, in a curved background with $\Gamma^{0}_{\nu\sigma}=0$ then $x^{0}=\zeta^{0}$ is not a solution. In many applications it is convenient to abandon the second gauge condition in $(16.4)$ and replace it by $\zeta^{0}=t$.
The string equation of motion is then
$$\frac{\partial}{\partial t}\left[ \frac{\dot{x}^{\mu}x'^{2}}{\sqrt{ -\gamma }} \right]+\frac{\partial}{\partial \zeta}\left[ \frac{x'^{\mu}\dot{x}^{2}}{\sqrt{ -\gamma }} \right]+\frac{1}{\sqrt{ -\gamma }}\Gamma^{\mu}_{\nu\sigma}(x'^2\dot{x}^{\nu}\dot{x}^\sigma+\dot{x}^2x'^{\nu}x'^\sigma)=0, \tag{17.2} $$where $\zeta=\zeta^{1}$. The new condition doesn't fix the gauge completely, we still have the freedom to perform transformations
$$\zeta\to \tilde{\zeta}(\zeta)\tag{17.3} .$$
Further simplification is possible for a static spacetime described by the metric
$$ds^2=f(\vec{x})dt^2+g_{ij}(\vec{x})dx^{i}dx^{j}.\tag{17.4} $$
In this metric, the $\mu=0$ component of $(17.2)$ is
$$\frac{\partial}{\partial t}\left[ f\left( -\frac{x'^2}{\dot{x}^2} \right)^{1/2} \right]=0.\tag{17.4} $$
Using the residual gauge freedom $(17.3)$ we can require
$$f\left( -\frac{x'^2}{\dot{x}^2} \right)^{1/2}=1.\tag{17.5} $$
Then the $\mu=i$ components of $(17.2)$ take the form
$$\partial_{t}(f^{-1}\dot{x}_{i})-\partial_{\zeta}(fx'_{i})+\frac{1}{2}g_{\nu\sigma,i}(f^{-1}\dot{x}^{\nu}\dot{x}^{\sigma}-fx'^{\nu}x'^{\sigma})=0.\tag{17.6} $$
The conserved energy of the string in static spacetime is
$$\mathcal{E}=\int d^3x\sqrt{ -g }T^{0}_{\;0}\tag{17.7} .$$
With the gauge conditions this reduces to
$$\mathcal{E}=\mu \int d\zeta\;f\left( -\frac{x'^2}{\dot{x}^2} \right)^{1/2}=\mu \int d\zeta,\tag{17.8} $$
where in the last step we have used $(17.5)$. From this we see that the choice of gauge corresponds to choosing the spacelike parameter $\zeta$ to be equal to the invariant length along the string, $\Delta \zeta=\Delta \mathcal{E}/\mu$.

For an expanding universe described by the [[Friedmann-Robertson-Walker Metric]], it is convenient to use conformal time $\tau$, $d\tau=dt/a(t)$, so that the metric takes the form
$$ds^2=a^2(\tau)(d\tau^2-d\vec{x}^2),\tag{17.9} $$
and the gauge conditions
$$\begin{matrix}
\zeta^{0}=\tau, & \dot{\vec{x}}\cdot \vec{x}'=0.
\end{matrix}\tag{17.10} $$
The equations of motion in this gauge can be obtained from $(17.2)$ or directly be varying the action $(15.7)$ with respect to $\vec{x}(\zeta,\tau)$,
$$\ddot{\vec{x}}+2 \frac{\dot{a}}{a}(1-\dot{\vec{x}}^2)\dot{\vec{x}}=\epsilon^{-1}(\epsilon^{-1}\vec{x}')',\tag{17.11} $$$$\dot{\epsilon}=-2 \frac{\dot{a}}{a}\epsilon \dot{\vec{x}}^2.\tag{17.12} $$
Here, dots and primes are derivatives with respect to conformal time $\tau$ and the spacelike parameter $\zeta$, respectively, and
$$\epsilon=\left( \frac{\vec{x}'^2}{1-\dot{\vec{x}}^2} \right)^{1/2}.\tag{17.13} $$
The string energy and momentum in an expanding universe can be defined as
$$\mathcal{E}=a(\tau)\mu \int d\zeta\;\epsilon,\tag{17.14} $$
$$\vec{P}=a(\tau)\mu \int d\zeta\;\epsilon \dot{\vec{x}}\tag{17.15} $$The rate of change of $\mathcal{E}$ and $\vec{P}$ can then be found using $(17.12)$,
$$\mathcal{\dot{E}}=\frac{\dot{a}}{a}(1-2\langle v^2\rangle)\mathcal{E},\tag{17.16} $$
$$\dot{\vec{P}}=-\frac{\dot{a}}{a}\vec{P},\tag{17.17} $$
where $\langle v^2 \rangle$ is the average string velocity squared,
$$\langle v^2 \rangle =\frac{{\int d\zeta\;\epsilon \dot{\vec{x}}}}{\int d\zeta\;\epsilon}\tag{17.18} .$$
Equation $(17.16)$ describes the manner in which the string will either gain energy through stretching or loose it through velocity redshifting. In flat space we have $\langle v^2 \rangle=\frac{1}{2}$ for any loop at rest, provided that this is time-averaged over one period. In the expanding universe, Hubble damping on large scales would be expected to reduce velocities somewhat, $\langle v^2 \rangle<\frac{1}{2}$, so stretching effects should dominate in $(17.16)$ is for large loops, $L \gtrsim d_{H}$. The damping term in $(17.11)$ is of order $(L/d_{H})^2$ and becomes increasingly less significant as the loop falls inside the horizon. For $L\ll d_{H}$ the evolution will be almost indistinguishable from that in flat space, and the energy of a loop will remain nearly constant. In this regime by $(17.17)$ the loop momentum will be redshifted like the momentum of a point particle in an expanding universe, $\vec{P}\propto a^{-1}$.

A static string, $\vec{x}(\zeta)=\vec{c}\zeta$ with $\vec{c}$ a constant, is a solution to $(17.11)$. A straight string remains straight and is simply stretched by expansion. For a moving string we can write
$$\vec{x}=\vec{b}(\tau)+\vec{c}\zeta \tag{17.19} ,$$with $\dot{\vec{b}}\cdot \vec{c}=0$  and $(17.11)$ gives
$$\dot{\vec{v}}+2\left( \frac{\dot{a}}{a} \right)(1-v^2)\vec{v}=0,\tag{17.20} $$
where $\vec{v}=\dot{\vec{b}}$ and $v=|\vec{v}|$. The solution of this equation is
$$v(1-v^2)^{-1/2}\propto a^{-2}\tag{17.21}. $$
Note that the string momentum per comoving volume decreases as $a^{-1}$, like the momentum of a loop. The difference between the two cases is that the mass of string per comoving volume grows as $a(\tau)$. Consider small perturbations on a static straight string. Representing $\vec{x}(\zeta,\tau)$ as
$$\vec{x}=\vec{c}\zeta+\delta \vec{x}\tag{17.22}, $$
we can linearise $(17.10-11)$ in $\delta \vec{x}$. For a power law expansion,
$$a(\tau)=\tau^{\alpha},\tag{17.23} $$
we have
$$\delta \ddot{\vec{x}}+\frac{2\alpha}{\tau}\delta \dot{\vec{x}}-\delta \vec{x}''=0,\tag{17.24} $$
$$\vec{c}\cdot\delta \dot{\vec{x}}=0,\tag{17.25} $$
where the parameter $\zeta$ has been chosen so that $|\vec{c}|=1$. The solution of $(17.24)$ which is well behaved as $\tau\to{0}$ is a superposition of waves of the form
$$\delta \vec{x}=\vec{A}\tau^{-\nu}J_{\nu}(k\tau)e^{ ik\zeta },\tag{17.26} $$
where $\nu=\alpha-\frac{1}{2}$ and the constant vector $\vec{A}$ is orthogonal to $\vec{c}$. $x^{i}$ are comoving coordinates so to obtain the physical wave parameters, $(17.26)$ has to be rescaled by $a(\tau)$. The physical wavelength is then $\lambda=2\pi a(\tau)/k$, which grows in proportion to the scale factor. The quantity $k\tau \sim t/\lambda$ gives the ratio of the horizon size to the wavelength, to an order of magnitude.
As $k\tau\to 0$, the time dependent factor in $(17.26)$ approaches a constant, which means that waves with $\lambda\gg t$ do not move in comoving coordinates. These waves are conformally stretched: both the amplitude and the wavelength grow like $a(\tau)$, while the shape of the string remains unchanged. In the opposite limiting case $k\tau\gg 1$, $\lambda\ll t$ the wavelength still grows as $a(\tau)$, but the physical amplitude of the wave, $a(\tau)\delta\vec{x}$ remains constant. As the ration of the amplitude to the wavelength decreases, the string progressively straightens. 
Numerical simulations of string evolution shows that the results of this perturbative analysis also apply for strongly curved strings. Waves on scales larger than the horizon are conformally stretched, while irregularities on scales below the horizon are smoothed out by the expansion.