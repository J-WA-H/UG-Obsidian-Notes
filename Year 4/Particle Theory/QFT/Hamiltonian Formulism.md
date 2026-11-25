We have a [Lagrangian](Classical%20Field%20Theory.md) $\mathcal{L}(\phi,\partial_{\mu }\phi)$ where $\phi$ is a generalised coordinate. From classical mechanics, its conjugate momentum is
$$\pi(x)=\frac{{\partial \mathcal{L}}}{\partial \dot{\phi}}\tag{3.1} $$where $\dot{\phi}=\partial_{0}\phi=\partial_{t}\phi$. This can be used to take a Legendre transform of the Lagrangian to give the Hamiltonian,
$$\mathcal{H}=\pi \dot{\phi}-\mathcal{L}.\tag{3.2} $$
It can be verified that $\frac{\partial \mathcal{H}}{\partial \dot{\phi}}=0$ so $\mathcal{H}$ does not depend on $\dot{\phi}$, so $\mathcal{H}=\mathcal{H}(\phi,\pi,\partial_{i}\phi)$ where $i=1,2,3$. In reality this is the Hamiltonian density, with the real Hamiltonian given by
$$H=\int d^3x\;\mathcal{H}.\tag{3.3} $$
Example: Real scalar free field theory. The Lagrangian is $(1.14)$
$$\mathcal{L}=\frac{1}{2}(\partial_{\mu}\phi)(\partial^\mu \phi)-\frac{1}{2}m^2\phi^2.\tag{1.14} $$
To take the Legendre transform, first need the conjugate momentum
$$\pi(x)=\frac{\partial \mathcal{L}}{\partial \dot{\phi}}=\partial_{t}\phi=\dot{\phi}.\tag{3.4} $$
This gives the Hamiltonian,
$$\mathcal{H}=\pi \dot{\phi}-\mathcal{L}=\pi^2-\frac{1}{2}(\partial_{\mu}\phi)(\partial^{\mu}\phi)+\frac{1}{2}m^2\phi^2=\frac{1}{2}\pi^2+\frac{1}{2}(\partial_{i}\phi)^2+\frac{1}{2}m^2\phi^2.\tag{3.5} $$
For a [[Complex Field Theory]], 
$$\mathcal{L}=(\partial_{\mu}\phi ^{*})(\partial^{\mu}\phi)-m^2\phi ^{*}\phi.\tag{2.1} $$
There are two fields so two conjugate momenta
$$\pi=\frac{\partial \mathcal{L}}{\partial \dot{\phi}}=\dot{\phi}^{*},\;\pi ^{*}=\frac{{\partial \mathcal{L}}}{\partial \dot{\phi}^{*}}=\dot{\phi}\tag{3.6}. $$
This gives the Hamiltonian
$$\mathcal{H}=\sum_{i}\pi_{i}\dot{\phi}_{i}-\mathcal{L}=\pi \pi ^{*}+\pi ^{*}\pi-\pi \pi ^{*}+|\partial_{i}\phi|^2+m^2|\phi|^2=\pi ^{*}\pi+|\partial_{i}\phi|^2+m^2|\phi|^2.\tag{3.7} $$
For a real scalar field theory, the Hamiltonian yields the [[Klein-Gordon Equation]]
$$(\partial^{\mu}\partial_{\mu}+m^2)\phi=0\tag{1.15} .$$
The general solution to this is
$$\phi(x)=\int \frac{d^3p}{(2\pi^3)2p_{0}} [a(p)e^{ -ip_{\mu}x^{\mu} }+a^{\dagger}(p)e^{ ip_{\mu}x^{\mu} }]_{p_{0}=\pm \sqrt{ |\vec{p}|^2+m^2 }\equiv E_{p}}.\tag{3.8} $$
The condition for $p_{0}$ is the mass-shell condition. Check it is a general solution:
$$(\partial_{\mu}\partial^{\mu}+m^2)\phi=\int \frac{d^3p}{(2\pi)^32p_{0}}[a(p)(-p_{\mu}p^{\mu}+m^2)e^{ -ip_{\mu}x^{\mu} }+a^{\dagger}(p)(-p_{\mu}p^{\mu}+m^2)e^{ ip_{\mu}x^{\mu} }]\tag{3.9} $$
$$=\int \frac{d^3p}{(2\pi)^32p_{0}}(-p_{\mu}p^{\mu})[a(p)e^{= ip_{\mu}x^{\mu} }+a^{\dagger}(p)e^{ ip_{\mu}x^{\mu} }]\tag{3.10}=0 $$since $p_{\mu}p^{\mu}=0$.
This shows this is a solution to the Klein-Gordon equation $\forall \;a,a^{\dagger}$ as it has two independent functions, $a,a^{\dagger}$, a feature of solutions of second order PDEs.

As $\phi(x)\in \mathbb{R}$, $\phi ^{*}=\phi \implies a^{*}=a^{\dagger}$ so $a,a^{\dagger}$ are not independent but complex conjugates of each other.

For a complex scalar field theory, replace $a^{\dagger}$ with a completely independent function $b^{\dagger}$,
$$\phi(x)=\int \frac{d^3p}{(2\pi)^32p_{0}}[a(p)e^{ -ip_{\mu}x^{\mu} }+b^{\dagger}(p)e^{ ip_{\mu}x^{\mu} }].\tag{3.11} $$
The integration measure is relativistically invariant,
$$\frac{d^3p}{(2\pi)^32p_{0}}=\frac{d^4p}{(2\pi)^4}(2\pi)\delta(p_{\mu}p^{\mu}-m^2)\tag{3.12} .$$For $p_{\mu}p^{\mu}-m^2=0$, $p_{0}=\pm E_{p}$ but we must take $+E_{p}$ so there is only 1 distinct solution.
