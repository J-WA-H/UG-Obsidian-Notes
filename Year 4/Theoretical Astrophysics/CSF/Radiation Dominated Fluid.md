Consider the change in the [sound speed](Baryon-Photon%20Fluid.md) at recombination. Just before, $c_{s}=1.3\times 10^{8}\text{ ms}^{-1}$ while just after, $c_{s}=6\times 10^{3}\text{ ms}^{-1}$. There is a sudden drop in $c_{s}$ due to the removal of the radiation pressure for baryons.

Due to this, the [[Jean's Length]], $\lambda_{J}\propto c_{s}$ drops by a factor of $2\times 10^{4}$. The Jeans mass, $M_{J}\propto c_{s}^3$ drops by a factor of $10^{13}$.

![[Pasted image 20251107114149.png]]

Before the matter-radiation epoch, the total energy density is dominated by radiation, $\rho \approx \rho_{r}>\rho_{m}$. Radiation, like a [[Baryon-Photon Fluid]], behaves as a relativistic fluid with
$$p=\frac{1}{3}\rho c^2;\;c_{s}=\frac{c}{\sqrt{ 3 }}\tag{15.1} .$$
Relativistic pressure requires modifications to [Newtonian fluid equations](Poisson's%20Equations.md).
Consider the relativistic Poisson equation,
$$\nabla^2\phi=4\pi G\left( \rho+\frac{3p}{c^2} \right)=8\pi G\rho.\tag{15.2} $$
The continuity equation is replaced by an energy conservation equation and the Euler equation uses a modified momentum balance. This means we need a new master equation,
$$\frac{\partial^2\delta}{\partial t^2}|_{\vec{x}}+2 \frac{\dot{a}}{a} \frac{\partial\delta}{\partial t}|_{\vec{x}}=\frac{\nabla^2_{\vec{x}}\delta p}{a^2\bar{\rho}}+\frac{32\pi G}{3} \bar{\rho}\delta.\tag{15.3} $$
The only difference is the self-gravity term that is larger by a factor of $\frac{8}{3}$.
There is a factor of 2 from the Poisson equation and a factor of $\frac{4}{3}$ from energy conservation.

For radiation domination, $\delta p=\frac{1}{3}c^2\delta \rho$ so
$$\frac{\partial^2\delta}{\partial t^2}+2 \frac{\dot{a}}{a} \frac{\partial\delta}{\partial t}=\frac{1}{3}c^2 \frac{\nabla^2\delta}{a^2}+\frac{32\pi G}{3}\bar{\rho}\delta.\tag{15.4} $$
This is very similar to a non-relativistic fluid. Assume a plane-wave solutions $\delta(\vec{x},t)=D(t)e^{ i\vec{k}\cdot \vec{x} }$.
$$\ddot{D}+2H(t)\dot{D}=\left( \frac{32}{3}\pi G\bar{\rho}(t)-\frac{c^2k^2}{3a^2} \right)D.\tag{15.5} $$
Define $k_{J}(t)$ s.t. $RHS=0$, 
$$k_{J}(t)=\left( \frac{32}{3}\pi G\bar{\rho}(t) \right)^{1/2} \frac{a(t)}{c_{s}}\tag{15.6} $$
$$\therefore\lambda_{J}(t)=\frac{2\pi}{k_{J}(t)}a(t)=\left( \frac{3\pi}{8} \right)^{1/2} \frac{c_{s}}{(G\bar{\rho})^{1/2}}.\tag{15.7} $$
$\lambda_{J}$ differs only by a factor of $\sqrt{ \frac{3}{8} }$ from the Newtonian case.

For $\lambda\gg\lambda_{J}$, $\nabla^2\delta p\approx0$ so
$$\frac{\partial^2\delta}{\partial t^2}+2 \frac{\dot{a}}{a} \frac{\partial\delta}{\partial t}-\frac{32\pi G}{3} \bar{\rho}\delta=0.\tag{15.8} $$
This is similar to the Newtonian equation for zero pressure, except for the $G\bar{\rho}\delta$ coefficient.

For a flat, radiation dominated universe,
$$a\propto t^{1/2},\;H=\frac{1}{2t},\;\bar{\rho}=\frac{3}{32\pi Gt^2}.\tag{15.9} $$
This gives the general solution,
$$\delta(\vec{x},t)=A(\vec{x})t+B(\vec{x})t^{-1}.\tag{15.10} $$
The growing mode is $D_{+}\propto t\propto a^2$, when for the matter dominated case, $D_{+}\propto t^{2/3}$,
![[Pasted image 20251107130045.png]]
