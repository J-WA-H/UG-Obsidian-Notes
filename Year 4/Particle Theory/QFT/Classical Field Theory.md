Quantum field theory is the union of quantum mechanics and special relativity, as quantum mechanics cannot describe particles with relativistic energies and special relativity doesn't describe quantum particles.

Classical field theory is the foundation for QFT, as the classical field is quantised to give a quantum field, and it is consistent with special relativity.

A field, $\phi(x)$, is a function of a spacetime variable $x=x_{\mu}=(t,\vec{x})$. Note that this course uses natural units $\hbar=c=e=1$.

A field is not a wavefunction but should be considered as a generalised coordinate.

There are three main types of fields:
- Scalar field $\phi(x)$ - after quantisation this describes spin-0 particles e.g. the Higgs boson. This is the simplest type of field.
- Dirac spinor field $\psi_{s}(x)$ - this describes spin-$\frac{1}{2}$ fermions e.g. electrons, positrons. $s=1,2,3,4$ is the spinor index, and the field is a 4D vector
$$\psi_{s}(x)=\begin{bmatrix}
\psi_{1}(x) \\
\psi_{2}(x) \\
\psi_{3}(x) \\
\psi_{4}(x)
\end{bmatrix}.\tag{1.1} $$
- Vector/gauge field $A_{\mu}(x)$ - describes spin-1 bosons e.g. photon from QED, gluon from QCD and $W^{\pm},Z^{0}$ from the standard model. These fields have the Lorentz index $\mu=0,1,2,3$

From classical mechanics, the Lagrangian is defined as
$$L(q(t),\dot{q}(t))=T-V\tag{1.2} $$where $q$ is a coordinate and $\dot{q}$ is the time derivative/velocity.
The Lagrangian can be used to derive the action
$$S=\int_{t_i}^{t_{f}}dtL(q,\dot{q}).\tag{1.3} $$
In classical mechanics the system evolves in such a way that $S$ is extremal - this is the principle of least action, given mathematically by
$$\delta S=0.\tag{1.4} $$
Extremising the action yields the Euler-Lagrange equations
$$\frac{{\partial L}}{\partial q}=\frac{d}{dt}\left( \frac{{\partial L}}{\partial \dot{q}} \right). \tag{1.5} $$The solution to this is the classical trajectory $q_{cl}(t)$.

The Hamilton formulism is another formulation of classical mechanics, where the Hamiltonian is defined by
$$H(q,p)=p\dot{q}-L(q,\dot{q})\tag{1.6} $$where $p$ is the coordinates conjugate momentum, defined by
$$p=\frac{{\partial L}}{\partial \dot{q}}.$$
It can be shown then that the Hamiltonian is a function of $q$ and $p$ but not $\dot{q}$. The Hamiltonian is also equivalent to the total energy
$$H=T+V.\tag{1.7} $$The principle of least action then yields the two Hamilton equations
$$\dot{q}=\frac{{\partial H}}{\partial p},\;\dot{p}=-\frac{{\partial H}}{\partial q}.\tag{1.8} $$
The scalar field can be written as $\phi(x_{\mu})=\phi(\vec{x},t)=\phi_{\vec{x}}(t)$, which has a continuous index $\vec{x}$ so we have a continuum of generalised coordinates. Similarly, $\dot{\phi}=\partial_{t}\phi(x)$

The Lagrangian can be written in terms of a Lagrangian density,
$$L=\int d^3x\mathcal{L}(\phi,\dot{\phi}).\tag{1.9} $$The Lagrangian density is formally defined as the difference between the kinetic and potential energy densities.

For simplicity, as $\mathcal{L}$ is used more often it is is simply known as just the Lagrangian.
Rewriting the action gives
$$S=\int dtL=\int d^4x\mathcal{L}(\phi,\partial_{\mu}\phi)\tag{1.10}. $$
To minimise this let $\phi(x)=\phi(x)+\alpha \varepsilon(x)$ while $\alpha$ is infinitesimally small. Substituting into the action gives
$$0=\frac{dS}{d\alpha}=\int d^4x\left( \frac{\partial \mathcal{L}}{\partial \phi} \frac{{\partial \phi}}{\partial \alpha}+\frac{{\partial \mathcal{L}}}{\partial(\partial_{\mu}\phi)} {\frac{\partial(\partial_{\mu}\phi)}{\partial\alpha}} \right).\tag{1.11} $$
where integrating by parts gives
$$\int d^4x\left[  \frac{{\partial \phi}}{\partial\alpha}\left( \frac{{\partial \mathcal{L}}}{\partial \phi}-\partial_{\mu} \frac{{\partial \mathcal{L}}}{\partial(\partial_{\mu}\phi)} \right)+\partial_{\mu}\left( \frac{{\partial \mathcal{L}}}{\partial(\partial_{\mu}\phi)} \frac{{\partial \phi}}{\partial\alpha} \right) \right]=0.\tag{1.12} $$
Given that the last term is a boundary term, it goes to zero which leaves the Euler-Lagrange equation
$$\frac{{\partial \mathcal{L}}}{\partial \phi}=\partial_{\mu}\left( \frac{{\partial \mathcal{L}}}{\partial(\partial_{\mu}\phi)} \right).\tag{1.13} $$
The simplest field theory model is a free real scalar field $\phi(x)$,
$$\mathcal{L}=\frac{1}{2}\partial^{\mu}\phi \partial_{\mu}\phi-\frac{1}{2}m^2\phi^2\tag{1.14} $$where $m$ is the mass of the field and $\phi\in \mathbb{R}$. This Lagrangian gives the [[Klein-Gordon Equation]],
$$(\partial^{\mu}\partial_{\mu}+m^2)\phi=0.\tag{1.15} $$
If the order of $\phi$ in the Lagrangian is $\mathcal{L}\sim \phi^2$, it is a free field theory but for $\mathcal{L}\sim \phi^{n>2}$ then this is an interacting field theory, e.g.
$$\mathcal{L}=\frac{1}{2}(\partial_{\mu}\phi)(\partial^{\mu}\phi)-\frac{1}{2}m^2\phi^2-\frac{\lambda}{4!}\phi^4.\tag{1.16} $$
In this Lagrangian, the standard free-field Lagrangian is given by $\mathcal{L}_{0}$ and the $\phi^4$ term is the interaction Lagrangian $\mathcal{L}_{int}$, with $\lambda$ a coupling constant.