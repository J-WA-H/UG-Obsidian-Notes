Assuming all perturbations are adiabatic so from [(8.6)](Fluid%20Perturbations.md),
$$\delta p=\left( \frac{\partial p}{\partial \rho} \right)_{ad}\delta \rho=c_{s}(t)^2\delta \rho.\tag{8.6} $$
This gives the [master equation](Linear%20Perturbation%20Equations.md),
$$\frac{\partial^2\delta}{\partial t^2}+2H(t) \frac{\partial\delta}{\partial t}=\frac{c_{s}^2(t)}{a^2(t)}\nabla^2\delta+4\pi G\bar{\rho}(t)\delta.\tag{12.1} $$
Like in the case [without pressure](Density%20Perturbations%20Without%20Pressure.md), all coefficients depend only on time.

Try separation of variables, $\delta(\vec{x},t)=D(t)F(\vec{x})$ where $F(\vec{x})$ is no longer arbitrary.

Separating the master equation gives
$$\frac{1}{F}\nabla^2F=-k^2\implies \nabla^2F=-k^2F\tag{12.2}. $$
This has plane-wave solutions,
$$F(\vec{x})\propto e^{ i\vec{k}\cdot \vec{x} }.\tag{12.3} $$
This gives the general solution
$$\delta(\vec{x},t)=D(t)e^{ i\vec{k}\cdot \vec{x} }.\tag{12.4} $$
$\vec{k}$ is the comoving wavenumber, related to comoving wavelength,
$$\lambda_{com}=\frac{2\pi}{k},\;k=|\vec{k}|.\tag{12.5} $$$\vec{k}$ and $\lambda_{com}$ remain constant in time.

The proper wavelength is
$$\lambda(t)=\lambda_{com}a(t)=\frac{2\pi}{k}a(t)\implies\lambda(t)\propto a(t).\tag{12.6} $$
For $D(t)$,
$$\ddot{D}+2H(t)\dot{D}=\left( 4\pi G\bar{\rho}(t)-\frac{c_{s}^2(t)k^2}{a^2(t)} \right)D=0\tag{12.7} $$using $\nabla^2(e^{ i\vec{k}\cdot \vec{x} })=-k^2e^{ i\vec{k}\cdot \vec{x} }$.

Using the Fourier transforms, arbitrary perturbations can be represented as a sum of plane waves. In linear theory, each of these plane waves evolves independently of all the others so solving for the evolution of the plane wave perturbations provides route to calculating evolution of general perturbations.

