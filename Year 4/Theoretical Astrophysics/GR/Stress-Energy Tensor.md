Considering [tidal forces](Newtonian%20Gravity%20and%20Curvature.md) $\frac{GM}{R^3}$, we get the mass density $\frac{M}{R^3}$. By saying gravity=curvature, we need a tensor equation. In relativity, mass is equivalent to energy so we could equivalently need the energy density.

In special relativity for single particles,
$$E=\gamma mc^2\tag{9.1} $$
have 4-velocity
$$u^\mu=\frac{dx^\mu}{d\tau}\tag{9.2} $$
which gives the 4-momentum
$$p^\mu=m u^{\mu}=m\begin{bmatrix}
c \\
0 \\
0 \\
0
\end{bmatrix}\tag{9.3}=\frac{dt}{d\tau}m\gamma \begin{bmatrix}
c \\
\frac{dx^1}{dt} \\
\frac{dx^2}{dt} \\
\frac{dx^3}{dt}
\end{bmatrix}. $$
Density requires multiple particles. Consider a number density
![[Pasted image 20260219120513.png]]
The number density of particles in the rest frame is $n_{0}$. Under a Lorentz boost, we get length contraction.

We get a flux of particles . Volume changes by length contraction $\gamma(u)$ so density increases, we also have a flux of particles leaving the box. This combines number density and particle flux. Define the number flux 4-vector $\vec{N}$,
$$\vec{N}=n_{0}\vec{u}\tag{9.4}$$
The components are $N^\mu=n_{0}u^\mu$. In the rest frame, $N^\mu=(c,0,0,0)=n_{0} \frac{dx^\mu}{d\tau}$.
In a moving frame,
$$N^\nu=n_{0} \frac{dx^\nu}{d\tau}=n_{0} \frac{dx^\nu}{dx^\mu} \frac{dx^\mu}{d\tau}=\frac{dx^\nu}{dx^\mu}N^\mu \tag{9.5}. $$
Extend this to the energy density. In the rest frame $\varepsilon=n_{0}mc^2=\rho_{0}c^2$. Transition to another frame, use the Lorentz transformation $\frac{dx^\nu}{dx^\mu}$. This means we need a second order tensor to describe energy density. Try combining them
$$T^{\mu \nu}=N^\mu p^\nu=n_{0}u^{\mu}u^{\nu}.\tag{9.6} $$
In the rest frame,
$$T^{00}=n_{0}mu^0u^0=n_{0}mc^2=\rho_{0}c^2\tag{9.7}. $$
The rest frame of dust assumes particles all have the same velocity. But we have thermal motions,
$$v\sim \sqrt{ \frac{k_{B}T}{m} }\tag{9.8} .$$In special relativity, the rest frame energy is $3P=3n_{0}k_{B}T$. The total energy density in the rest frame is then
$$n_{0}mc^2+3P=n_{0}mc^2+3n_{0}k_{B}T\tag{9.9}. $$
If $T^{\mu \nu}=\mathrm{diag}(\rho_{0}c^2,P,P,P)$, this gives the rest energy density and 3 tomes the pressure. This can be obtained by using
$$T^{\mu \nu}=\left( \rho_{0}+\frac{P}{c^2} \right)u^\mu u^\nu-P\eta^{\mu \nu}\tag{9.10} $$
with the Minkowski metric $\eta^{\mu \nu}=\mathrm{diag}(1,-1,-1,-1)$, $ds^2=\eta_{\mu \nu}dx^\mu dx^\nu$, $dx^{0}=cdt$.
$$\therefore T^{00}=\left( \rho_{0}+\frac{P}{c^2} \right)c^2-P\eta^{00}=\rho_{0}c^2+P-P=\rho_{0}c^2\tag{9.11}. $$
$$T^{11}=\left( \rho_{0}+\frac{P}{c^2} \right)0-P(-1)=P\tag{9.12} $$
which also holds for $T^{22}=T^{33}$. This is a perfect fluid stress-energy tensor.

This shows pressure contributes to the energy density.

- $T^{00}$ represents the energy density
- $T^{0i}$ represents energy flux through the $i^{th}$ surface
- $T^{i{0}}$ represents momentum density, which corresponds to energy flux
- $T^{ij}$ for $i\neq j$ represents shear forces, 0 for a perfect fluid.

For conservation laws, we need to consider how $T^{\mu \nu}$ conserves energy,
![[Pasted image 20260221104332.png]]
The energy in the box is $\ell^3T^{00}$. The rate of change of energy is $\ell^3 \frac{\partial T^{00}}{\partial t}$. The energy flow in the $yz$ plane is
$$\ell^2(T^{01}(x)-T^{01}(x+\ell))=\ell^2c \frac{\partial T^{01}}{\partial x}\ell=\ell^3c \frac{\partial T^{01}}{\partial x}\tag{9.13}. $$
Counting all surfaces gives
$$\frac{\ell^3}{c} \frac{\partial T^{00}}{\partial t}=-\ell^3 \frac{\partial T^{01}}{\partial x}-\ell^3 \frac{\partial T^{02}}{\partial y}-\ell^3 \frac{\partial T^{03}}{\partial z}\tag{9.14} \implies \frac{\partial T^{00}}{\partial x^0}+\frac{\partial T^{0i}}{\partial x^i}=0.$$
Combining these gives
$$\partial_{\alpha}T^{0\alpha}=0\tag{9.15}. $$
This shows conservation of energy. Conservation of momentum is given by
$$\partial_{\alpha}T^{i\alpha}=0\tag{9.16} ,$$
which, combining into one equation gives the conservation of energy and momentum,
$$\partial_{\alpha}T^{\beta\alpha}=0\tag{9.17}. $$
