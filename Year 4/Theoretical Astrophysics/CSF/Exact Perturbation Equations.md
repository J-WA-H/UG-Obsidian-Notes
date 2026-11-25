We can transform the [[Fluid Equations]] from proper to [comoving coordinates](Cosmological%20Expansion.md) which leads to simpler equations for [perturbed quantities](Fluid%20Perturbations.md). Comoving coordinates means they are unperturbed by Hubble flow.

To derive these transformations, consider the 1D case, $(r,t)\to(x,t)$ where $x\equiv \frac{r}{a(t)}$ is the comoving distance and $r$ is the proper distance. For some function $f(x,t)$,
$$\frac{\partial f}{\partial t}|_{r}=\frac{\partial f}{\partial x}|_{t} \frac{\partial x}{\partial t}|r+\frac{\partial f}{\partial t}|_{x} \tag{9.1} $$
$$\frac{\partial x}{\partial t}|_{r}=-\frac{\dot{a}}{a^2}r=-\frac{\dot{a}}{a}\implies \frac{\partial f}{\partial t}|_{r}=-\frac{\dot{a}}{a}x \frac{\partial f}{\partial x}|_{t}+\frac{\partial f}{\partial t}|_{x}\tag{9.2}. $$
For the spatial derivative,
$$\frac{\partial f}{\partial r}|_{t}=\frac{\partial f}{\partial x}|_{t} \frac{\partial x}{\partial r}|_{t}+\frac{\partial f}{\partial t}|_{x} \frac{\partial t}{\partial r}|_{t}\tag{9.3} .$$
$$\frac{\partial x}{\partial r}|_{t}=\frac{1}{a(t)};\; \frac{\partial t}{\partial r}|_{t}=0\implies \frac{\partial f}{\partial r}|_{r}=\frac{1}{a} \frac{\partial f}{\partial x}|_{t}.\tag{9.4} $$
These can be generalised to 3D,
$$\frac{\partial}{\partial t}|_{\vec{r}}=\frac{\partial}{\partial t}_{\vec{x}}-\frac{\dot{a}}{a}\vec{x}\cdot \vec{\nabla}_{\vec{x}},\;\vec{\nabla}_{\vec{r}}=\frac{1}{a}\vec{\nabla}_{\vec{x}}.\tag{9.5} $$
Consider perturbations to uniform expanding fluids (not necessarily small). The density is given by
$$\rho(\vec{r},t)=\bar{\rho}+\delta \rho(\vec{r},t)=\bar{\rho}[1+\delta(\vec{r},t)]\tag{9.6} $$where $\delta$ is the fractional density perturbation,
$$\delta\equiv \frac{\delta \rho}{\bar{\rho}}.\tag{9.7} $$
The perturbed velocity is given by
$$\vec{u}(\vec{r},t)=H\vec{r}+\vec{v}=\left( \frac{\dot{a}}{a} \right)\vec{r}+\vec{v}\tag{9.8} $$where $\vec{v}=\vec{v}(\vec{r},t)$ is the velocity perturbation (peculiar velocity).

The perturbed gravitational potential is
$$\Phi(\vec{r},t)=\frac{2\pi G}{3}\bar{\rho}(t)|\vec{r}|^2+\phi \tag{9.9} $$where $\phi=\phi(\vec{r},t)$ is the gravitational potential perturbation (peculiar gravitational potential).

The perturbed pressure is given by
$$p(\vec{r},t)=\bar{p}(t)+\delta p(\vec{r},t).\tag{9.10} $$
These can be used to determine the exact perturbation equations. We have the continuity equation $(5.12)$,
$$\frac{\partial \rho}{\partial t}|_{\vec{r}}+\vec{\nabla}_{\vec{r}}\cdot(\rho \vec{u})=0.\tag{5.12} $$
Substitute in the perturbed quantities:
$$\frac{\partial}{\partial t}|_{\vec{r}}(\bar{\rho}(t)(1+\delta))+\vec{\nabla}_{\vec{r}}\cdot\left[ \bar{\rho}(t)(1+\delta)\left( \frac{\dot{a}}{a}\vec{r}+\vec{v} \right) \right]=0\tag{9.11} $$
$$\implies \bar{\rho} \frac{\partial}{\partial t}|_{\vec{r}}(1+\delta)+(1+\delta)\dot{\bar{\rho}}+\bar{\rho}\vec{\nabla}_{\vec{r}}\cdot\left[ \frac{\dot{a}}{a}\vec{r}+\delta\frac{\dot{a}}{a}\vec{r}+(1+\delta)\vec{v} \right]=0\tag{9.12} $$
$$\implies \bar{\rho} \frac{\partial\delta}{\partial t}|_{\vec{r}}+\dot{\bar{\rho}}\delta+\dot{\bar{\rho}}+\bar{\rho}\vec{\nabla}_{\vec{r}}\cdot\left[ \frac{\dot{a}}{a}\vec{r} \right]+\bar{\rho}\vec{\nabla}_{\vec{r}}\cdot\left[ \delta  \frac{\dot{a}}{a}\vec{r}+(1+\delta)\vec{v} \right]=0\tag{9.13} .$$Terms for the background solution satisfy continuity equation so they cancel. Using $\dot{\bar{\rho}}=-3 \frac{\dot{a}}{a}\bar{\rho}$ gives
$$\frac{\partial\delta}{\partial t}|_{\vec{r}}-3 \frac{\dot{a}}{a}\delta+\vec{\nabla}_{\vec{r}}\cdot\left[ \delta  \frac{\dot{a}}{a}\vec{r}+(1+\delta)\vec{v} \right]=0\tag{9.14}. $$
Using the vector identity $\vec{\nabla}\cdot(f\vec{u})=\vec{u}\cdot \vec{\nabla}f+f\vec{\nabla}\cdot \vec{u}$,
$$\frac{\partial\delta}{\partial t}|_{\vec{r}}+\frac{\dot{a}}{a}\vec{r}\cdot \vec{\nabla}_{\vec{r}}\delta+\vec{\nabla}_{\vec{r}}\cdot[(1+\delta)\vec{v}]=0\tag{9.15} .$$
Changing from proper to comoving coordinates gives
$$\frac{\partial\delta}{\partial t}|_{\vec{x}}+\frac{1}{a}\vec{\nabla}_{\vec{x}}\cdot[(1+\delta)\vec{v}]=0.\tag{9.16} $$
This is the exact perturbed continuity equation for the time evolution of the fractional density perturbation $\delta$.

The same process can be used to derive the exact Euler equation, starting with $(5.20)$,
$$\frac{\partial \vec{u}}{\partial t}|_{\vec{r}}+(\vec{u}\cdot \vec{\nabla}_{\vec{r}})\vec{u}=-\frac{\vec{\nabla}_{\vec{r}}p}{\rho}-\vec{\nabla}_{\vec{r}}\Phi \tag{5.20} .$$
Substitute perturbated quantities,
$$\frac{\partial}{\partial t}|_{\vec{r}}\left( \frac{\dot{a}}{a}\vec{r}+\vec{v} \right)+\left( \frac{\dot{a}}{a}\vec{r}+\vec{v} \right)\cdot \vec{\nabla}_{\vec{r}}\left( \frac{\dot{a}}{a}\vec{r}+\vec{v} \right)=-\frac{\vec{\nabla}_{\vec{r}}(\bar{p}+\delta p)}{\bar{\rho}(1+\delta)}-\vec{\nabla}_{\vec{r}}\left( \frac{2\pi G}{3}\bar{\rho}|\vec{r}|^2+\phi \right).\tag{9.17} $$
Using $\vec{\nabla}_{\vec{r}}p=0$,
$$\frac{\partial}{\partial t}|_{\vec{r}}\left( \frac{\dot{a}}{a}\vec{r} \right)+\frac{\partial \vec{v}}{\partial t}|_{\vec{r}}+\frac{\dot{a}}{a}\vec{r}\cdot \vec{\nabla}_{\vec{r}}\left( \frac{\dot{a}}{a}\vec{r} \right)+\frac{\dot{a}}{a}\vec{r}\cdot \vec{\nabla}_{\vec{r}}\vec{v}+\vec{v}\cdot \vec{\nabla}_{\vec{r}}\left( \frac{\dot{a}}{a}\vec{r} \right)+\vec{v}\cdot\vec{\nabla}_{\vec{r}}\vec{v}=-\frac{\vec{\nabla}_{\vec{r}}\delta p}{\bar{\rho}(1+\delta)}-\vec{\nabla}_{\vec{r}}\left( \frac{2\pi G}{3}\bar{\rho}|\vec{r}|^2 \right)-\vec{\nabla}_{\vec{r}}\phi.\tag{9.18} $$
Simplifying this using the background solutions gives
$$\frac{\partial \vec{v}}{\partial t}|_{\vec{r}}+\frac{\dot{a}}{a}\vec{r}\cdot \vec{\nabla}_{\vec{r}}\vec{v}+\vec{v}\cdot \vec{\nabla}_{r}\left( \frac{\dot{a}}{a}\vec{r} \right)+\vec{v}\cdot \vec{\nabla}_{\vec{r}}\vec{v}=-\frac{\vec{\nabla}_{\vec{r}}\delta p}{\bar{\rho}(1+\delta)}-\vec{\nabla}_{\vec{r}}\phi.\tag{9.19} $$
Using $(\vec{v}\cdot \vec{\nabla}_{\vec{r}})\vec{r}=\vec{v}$ and moving to comoving coordinates gives the exact Euler equation,
$$\frac{\partial \vec{v}}{\partial t}|_{\vec{x}}+\frac{\dot{a}}{a}\vec{v}+\frac{1}{a}(\vec{v}\cdot \vec{\nabla}_{\vec{x}})\vec{v}=-\frac{\vec{\nabla}_{\vec{x}}\delta p}{a\bar{\rho}(1+\delta)}-\frac{\vec{\nabla}_{\vec{x}}\phi}{a}.\tag{9.20} $$
Applying the same method to the Poisson equation $(6.4)$,
$${\nabla}^2_{\vec{r}}\Phi=4\pi G\rho.\tag{6.4} $$Substitute perturbed quantities,
$$\nabla^2_{\vec{r}}\left( \frac{2\pi G}{3}\bar{\rho}r^2+\phi \right)=4\pi G\bar{\rho}(1+\delta)\implies \nabla^2_{\vec{r}}\phi=4\pi G\bar{\rho}\delta.\tag{9.21} $$
Moving into comoving coordinates gives the exact Poisson equation
$$\nabla^2_{\vec{x}}\phi=4\pi Ga^2\bar{\rho}\delta.\tag{9.22} $$
