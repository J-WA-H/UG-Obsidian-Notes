To treat cosmology in full generality requires general relativity however the Newtonian [[Fluid Equations]] are a good approximation when:
- $u\ll c$ - the size of Hubble expansion is $u=Hr$, this requires $r\ll \frac{c}{H}$
- $p\ll \rho c^2$ non-relativistic pressure - doesn't hold for radiation dominated fluid, $p=\frac{1}{3}\rho c^2$
- Negligible spatial curvature - if $|1-\Omega|\ll 1$, this guarantees $r\ll \frac{c}{H}$.

All fluid equations are expressed in proper coordinates $(\vec{r},t)$ - a coordinate system in fixed space with distances in physical units, so
$$\vec{\nabla}=\vec{\nabla}_{\vec{r}}=\left( \frac{\partial}{\partial x}, \frac{\partial}{\partial y}, \frac{\partial}{\partial x} \right)_{t}\tag{7.1} $$
$$\frac{\partial}{\partial t}=\frac{\partial}{\partial t}|_{\vec{r}}\tag{7.2} .$$
The aim is to show that an expanding universe is a solution of the Newtonian fluid equations.

First, define comoving coordinate $\vec{x}$,
$$\vec{x}=\frac{\vec{r}}{a(t)}\tag{7.3} .$$
For a uniform density expanding fluid, $\rho=\rho(t)$ and all fluid elements have constant $\vec{x}$ so
$$\vec{u}= \vec{\dot{r}}=\dot{a}\vec{x}=\frac{\dot{a}}{a}\vec{r}=H\vec{r}\tag{7.4} .$$
First consider continuity equation:
$$\frac{\partial \rho}{\partial t}|_{\vec{r}}+\vec{\nabla}_{\vec{r}}\cdot(\rho \vec{u})=0\tag{7.5} .$$Using $\vec{u}=\frac{\dot{a}}{a}\vec{r}$,
$$\frac{d\rho}{dt}+\vec{\nabla}_{\vec{r}}\cdot\left( \rho(t) \frac{\dot{a}}{a}\vec{r} \right)=0\tag{7.6} $$
$$\implies \dot{\rho}+3\rho\frac{ \dot{a}}{a}=0,\tag{7.7} $$
since $\vec{\nabla}\cdot \vec{r}=3$. This yields solutions $\rho(t)\propto a^{-3}(t)$, which shows the conservation of rest mass in an expanding universe.

For the Poisson equation - use the fact that the universe is homogeneous and isotropic, $\Phi(\vec{r},t)=\Phi(r,t)$,
$$\therefore \nabla^2_{r}\Phi=\frac{1}{r^2} \frac{\partial}{\partial r}\left( r^2 \frac{\partial \Phi}{\partial r} \right)=4\pi G\rho(t)\tag{7.8} $$
$$\implies \Phi(r,t)=\frac{2\pi G}{3}\rho(t)r\tag{7.9}+\text{const}. $$
Also
$$\vec{g}=-\vec{\nabla} \Phi=-\frac{4\pi G}{3}\rho(t)\vec{r}.\tag{7.10} $$
For the Euler equation,
$$\frac{\partial \vec{u}}{\partial t}+(\vec{u}\cdot \vec{\nabla})\vec{u}=-\frac{1}{\rho}\vec{\nabla}p-\vec{\nabla}\Phi \tag{5.20} $$For the left hand side substitute $\vec{u}$, 
$$\frac{\partial}{\partial t}\left( \frac{\dot{a}}{a}\vec{r} \right)+\frac{\dot{a}}{a}(\vec{r}\cdot \vec{\nabla})\left( \frac{\dot{a}}{a} \right)\vec{r}=\frac{\ddot{a}}{a}\vec{r}.\tag{7.11} $$
For the right hand side, $p=p(t)$ so $\vec{\nabla}p=0$.
$$\therefore \frac{\ddot{a}}{a}=-\frac{4\pi G}{3}\rho(t)\tag{7.12} $$
This is the Newtonian Friedmann acceleration equation without relativistic effects.
Integrating this and using $\rho=\rho_{0}/a^3$ gives
$$\left( \frac{\dot{a}}{a} \right)^2=\frac{8\pi G\rho}{3}+\frac{B}{a^2},\tag{7.13} $$where $B$ is a constant of integration, which from general relativity gives $B=-kc^2$.

This shows that the uniform density expanding universe is an exact solution to the Newtonian fluid equations.