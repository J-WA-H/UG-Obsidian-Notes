The gravitational field of a straight string has no Newtonian force, which can be understood from linear perturbation theory [(19.3-5)](Linearised%20Gravity.md). The source of the Newtonian potential $\Phi=\frac{1}{2}h_{00}$, is
$$S_{00}=S^{0}_{\;0}=\frac{1}{2}(T^0_{\;0}-T^i_{\;i}).\tag{22.1} $$
For the energy-momentum tensor [(16.12)](Strings%20in%20Flat%20Spacetime.md) of a string we have
$$S^{0}_{\;0}(\vec{r},t)=\mu \int d\zeta \dot{\vec{x}}^2\delta^{(3)}(\vec{r}-\vec{x}(\zeta,t)).\tag{22.2} $$
In the rest frame of a straight string, $S^{0}_{\;0}=0$ and the gravitational potential vanishes. A string can be static only if it is straight, and so curved strings produce non-zero gravitational potentials. 

The retarded solution of the wave equation $(19.4)$ can be written as
$$h^{\mu \nu}(\vec{r},t)=-4G\int \frac{d^3y}{|\vec{r}-\vec{y}|}S^{\mu \nu}(\vec{r},t-|\vec{r}-\vec{y}|).\tag{22.3} $$
Using $(19.5)$ and $(19.7)$ and integrating over $\vec{y}$ gives
$$h^{\mu \nu}(\vec{r},t)=-4G\mu \int \frac{F^{\mu \nu}(\zeta,\tau)d\zeta}{|\vec{r}-\vec{x}(\zeta,\tau)||(1-\hat{n}\cdot \dot{\vec{x}}(\zeta,\tau))|},\tag{22.4} $$
where
$$\hat{n}=\frac{{\vec{r}-\vec{x}(\zeta,\tau)}}{|\vec{r}-\vec{x}(\zeta,\tau)|},\tag{22.5} $$
$$F^{\mu \nu}=\dot{x}^{\mu}\dot{x}^{\nu}-x'^{\mu}x'^{\nu}+\eta^{\mu \nu}x'^{\sigma}x'_{\sigma},\tag{22.6} $$
and the retarded time given by
$$\tau=t-|\vec{r}-\vec{x}(\zeta,\tau)|.\tag{22.7} $$
