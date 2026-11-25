Consider the [[Abelian Higgs Model]]. To estimate the interaction energy of a stationary multi-vortex configuration, suppose the true solutions $(\Phi,\vec{A})$ can be accurately approximated by a superposition of individual cylindrically symmetric $n=1$ vortex solutions $(\hat{\Phi},\hat{A})$ provided the vortex zeros are widely separated. The $n$-vortex solution with zeros at points $\vec{r}_{k}$ will then be given by the ansatz
$$\hat{\Phi}(\vec{r})=\prod_{k=1}^{n}\phi_{k}(\vec{r})=\prod_{k=1}^{n}\phi_{s}(\vec{r}-\vec{r}_{k})\tag{12.1} $$
$$\hat{A}(\vec{r})=\sum_{k=1}^{n}\vec{A}_{k}(\vec{r})=\sum_{k=1}^{n}\vec{A}_{s}(\vec{r}-\vec{r}_{k}).$$
To evaluate the potential between the two vortices, the asymptotic accuracy of these fields must be established for large separations, $d\gg m_{s}^{-1},m_{v}^{-1}$. The true fields in terms of the residual fields $(\varphi,\vec{a})$ are
$$\begin{matrix}
\Phi=\hat{\Phi}+\varphi, & \vec{A}=\hat{A}+\vec{a}.
\end{matrix}\tag{12.2} $$We require that the additional contribution $\epsilon_{\varphi,\vec{a}}(\hat{\Phi},\hat{A})$ to the vortex energy be negligible,
$$\mu(\Phi,\vec{A})=\mu(\hat{\Phi},\hat{A})+\epsilon_{\varphi,\vec{a}}(\hat{\Phi},\hat{A}).\tag{12.3} $$
We can represent the left-hand side of the field equation $(10.7)$ in the form $L_{\phi}(\phi,\vec{A})$. For an $n=2$ vortex configuration, the substitution of the ansatz $\hat{\Phi},\hat{A}$ gives the field equation
$$L_{\phi}(\hat{\Phi},\hat{A})=\phi_{1}L_{\phi}(\phi_{2},\vec{A}_{2})+\phi_{2}L_{\phi}(\phi_{1},\vec{A}_{1})+\mathcal{O}(\exp[-\sqrt{ 2 }ed]),\tag{12.4} $$
because of the asymptotic fall-off of the individual solutions $(\phi_{i},\vec{A}_{i})$. This assumes we are in the type II regime with $\beta>1$. Similarly, the field equation $(10.8)$ shows that the gauge field equations are accurate to $\vec{L}_{\vec{A}}(\hat{\Phi},\hat{A})\approx \mathcal{O}(\exp[-\sqrt{ 2 }ed])$. These expressions imply that the residual fields behave as $\varphi,\vec{a}\approx \mathcal{O}(\exp[-\sqrt{ 2 }ed])$, so it can be easily verified that the residual energy consists entirely of terms of second order or higher
$$\epsilon_{\varphi,\vec{a}}(\hat{\Phi},\hat{A})\approx \mathcal{O}(\exp[-2\sqrt{ 2 }ed]).\tag{12.5} $$
This is an important result for creating string configurations as initial data for dynamical numerical simulations. To evaluate the energy of the two vortices, the expression is split into that of the free solutions plus an overlap integral,
$$E(\hat{\Phi},\hat{A})\approx{2}\mu(\phi_{1},\vec{A}_{1})+E_{int}(\hat{\Phi},\hat{A})\tag{12.6}. $$
Using the asymptotic properties of the vortex solutions, it can be shown that each contribution to $E_{int}(\hat{\Phi},\hat{A})$ is of the order $\mathcal{O}(\exp[-\sqrt{ 2 }ed])$. For strong type II behaviour, $\beta\gg 1$, this overlap integral can be approximated as
$$E_{int}(\hat{\Phi},\hat{A})\approx\left( \frac{\sqrt{ 2 }\pi^{3}}{ed} \right)^{1/2}\exp[-\sqrt{ 2 }ed],\tag{12.7} $$
indicating that at large distances vortices repel each other with an exponentially decreasing force. This repulsion force confirms the expectation for type II behaviour where vector field effects dominate.
The covariant derivative term provides a negative contribution to the overlap integral, suggesting that the attraction from the scalar field might be greater for $\beta<1$, below critical coupling at which the interaction energy vanishes.  The interaction energy is repeated for a vortex-antivortex pair but the magnetic flux cancels, the vector contribution is now also attractive so the vortex and antivortex always attract at large distances with an exponentially small force. Vortices only have short-range Yukawa-type interactions so local $U(1)$-strings in three dimensions are non-interacting except when the strings intersect.

The derivation for the vortex-antivortex interaction can also be repeated for global $U(1)$-strings. Take the ansatz
$$\hat{\Phi}=\phi_{s}(\vec{r}-\vec{r}_{1})\bar{\phi}_{2}(\vec{r}-\vec{r}_{2})\tag{12.8} $$
which is the product of two isolated axisymmetric solutions. At large fixed separation $(12.8)$ will closely approximate the minimum energy configuration. From the field equation $(10.25)$ we can estimate that $L_{\phi}\lesssim\mathcal{O}(d^{-1})$ with the residual field $\varphi\lesssim\mathcal{O}(d^{-1})$, and hence the residual energy is
$$\epsilon_{\varphi}(\hat{\Phi})\lesssim\mathcal{O}(d^{-1}).\tag{12.9}$$
Subtracting the individual vortex energy densities [(7.6)](Cosmic%20Strings) yields the axisymmetric interaction energy density 
$$\mathcal{E}^{\pm}_{int}\approx\pm 2\eta^2 \frac{{r^2-d^2}}{(r^2+d^2)^2},\tag{12.10} $$
where the upper sign is for a vortex-vortex pair and the lower for a vortex-antivortex pair. Assuming a cut-off distance $R\gg d\gg\delta$ this can be integrated to give
$$E^{\pm}_{int}(\hat{\Phi})\approx \pm 4\pi \eta^2\ln\left( \frac{R}{d} \right),\tag{12.11} $$ from which we can obtain the inter-vortex force, $F=-\partial E^{\pm}/\partial d$,
$$F\approx\pm \frac{4\pi \eta^2}{d}. \tag{12.12} $$
This implies that two vortices feel a strong repulsive force and we can expect an $n>1$ global vortex configuration to be unstable. On the other hand, a vortex-antivortex pair will feel a strong attraction, being effectively confined. These long-range interactions are due to a massless Goldstone boson in the model, and indicate that global and local string dynamics will differ substantially. 