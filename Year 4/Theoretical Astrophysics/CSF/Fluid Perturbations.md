Fluid perturbations can be sound waves moving through an ideal gas.

Consider an ideal gas with no gravity. The background solution is a uniform gas density at rest, i.e. $\rho=\bar{\rho}$, $\vec{u}=0$. Introduce perturbations $\delta \rho\ll \bar{\rho}$, $\delta p\ll \bar{p}$,
$$\begin{matrix}
\rho(\vec{r},t)=\bar{\rho}+\delta \rho(\vec{r},t) & p(\vec{r},t)=\bar{p}+\delta p(\vec{r},t)
\end{matrix}.\tag{8.1} $$
The fluid velocity $\vec{u}$ is also a perturbation, $\vec{u}(\vec{r},t)=\delta \vec{u}(\vec{r},t)$ since $\bar{u}=0$.

Recall the [continuity equation](Fluid%20Equations.md) and substitute in $\bar{\rho}+\delta \rho(\vec{r},t)$,
$$\frac{\partial(\delta \rho)}{\partial t}+\bar{\rho}\vec{\nabla}\cdot \vec{u}+\vec{\nabla}\cdot\cancelto{0}{(\delta \rho \vec{u})}=0.\tag{8.2} $$
This assumes that and 2nd order perturbations are negligible.
Discarding terms higher than 1st order in perturbed quantities gives
$$\frac{\partial(\delta \rho)}{\partial t}+\bar{\rho}\vec{\nabla}\cdot \vec{u}=0.\tag{8.3} $$
For the Euler equation, use the fact there is no gravity so $\Phi=0$,
$$\frac{\partial \vec{u}}{\partial t}+\cancelto{0}{(\vec{u}\cdot \vec{\nabla})\cdot \vec{u}}=-\frac{\vec{\nabla}(\delta p)}{(\bar{\rho}+\delta \rho)}\approx-\left( 1-\frac{\delta p}{\rho} \right) \frac{\vec{\nabla}(\delta p)}{\bar{\rho}}\tag{8.4} .$$
Discarding higher order terms gives
$$\frac{\partial \vec{u}}{\partial t}=-\frac{\vec{\nabla}(\delta p)}{\bar{\rho}}\tag{8.5} $$
with $p=K(S)\rho^{\gamma}$ and for adiabatic changes, $\delta S=0$ to first order,
$$\delta p=\frac{\gamma \bar{p}}{\bar{\rho}}\delta \rho=c_{s}^2\delta \rho \tag{8.6} $$where the sound speed is given by
$$c_{s}^2=\left( \frac{\partial p}{\partial \rho} \right)_{ad}=\left( \frac{\gamma \bar{p}}{\bar{\rho}} \right).\tag{8.7} $$
The perturbed Euler equation becomes
$$\frac{\partial \vec{u}}{\partial t}=-\frac{\vec{\nabla}(\delta p)}{\bar{\rho}}=-c_{s}^2 \frac{\vec{\nabla}(\delta p)}{\bar{\rho}}\tag{8.8} $$with the perturbed continuity equation $(8.3)$ and recalling $\vec{\nabla}\cdot(\vec{\nabla}f)=\nabla^2f$ we get
$$\frac{\partial^2(\delta \rho)}{\partial t^2}=c_{s}^2\nabla^2(\delta \rho)\tag{8.9}. $$This is a wave equation for perturbations $\delta \rho(\vec{r},t)$ with wave speed $c_s$.