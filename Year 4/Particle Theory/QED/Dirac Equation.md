The [Klein-Gordon equation](Classical%20Field%20Theory.md) uses the equation of motion
$$(E^2-p^2-m^2)\phi=0\tag{1.1}. $$
This admits negative energy solutions, however, this is fixed by the interpretation that the particle is moving backwards in time, which is an antiparticle. This moves the minus sign from the energy to time.

The bigger issue is the negative probability density,
$$\rho=j^{0}=(\partial_{t}\phi ^{*})\phi-\phi ^{*}(\partial_{t}\phi)\propto-2ik_{0}.\tag{1.2} $$
To normalise this, shift $j^{0}\to \frac{j^{0}}{2m}$. The negative probability density comes from the $E^2$ term as its square root gives a positive and negative term.

Dirac decided to solve this by linearising the Klein-Gordon equation,
$$i \frac{\partial \psi}{\partial t}+i\vec{\alpha}\cdot \vec{\nabla}\psi-\beta m\psi=0.\tag{1.3} $$Squaring this operator gives the Klein-Gordon equation. 
$\alpha,\beta$ are matrices so we write $\psi$ as a 4-component object like a vector. Note that these spinors are not vectors as they don't transform like vectors under a Lorentz transformation.

In index notation, this is
$$i \frac{\partial \psi_{i}}{\partial t}+i\vec{\alpha}_{ij}\cdot \vec{\nabla}\psi_{j}-\beta_{ij}m\psi_{j}=0\tag{1.4} $$where $i,j$ are Dirac indices.
$\alpha_{ij},\beta_{ij}$ are traceless objects, $\mathrm{Tr}[\alpha_{i}]=\mathrm{Tr}(\beta)=0$, to avoid derivatives mixing. $\vec{\alpha}$ is a vector of matrices $\alpha_{i}$.

The anticommutator relations are
$$\alpha_{i}\alpha_{j}+\alpha_{j}\alpha_{i}=\{ \alpha_{i},\alpha_{j} \}=2\delta_{ij},\;\{ \alpha_{i},\beta \}=0.\tag{1.5} $$
$\alpha_{i}^2=\beta^2=\mathbb{I}$. All these conditions indicate the matrices have even dimensions.

If we work in two dimensions, we can ignore $\beta$ as there are only linearly independent matrices that satisfy the conditions are the Pauli matrices.
In 2 dimensions, we have the Weyl spinor which gives $m\equiv 0$.
In 4 dimensions, we have the Dirac spinor which gives $m\neq 0$.

These matrices can be given by the gamma matrices $\gamma^{\mu}$,
$$\gamma^{0}=\begin{bmatrix}
\mathbb{I} & 0 \\
0 & -\mathbb{I}
\end{bmatrix},\;\gamma^{i}=\beta\alpha_{i}=\begin{bmatrix}
0 & \sigma_{i} \\
-\sigma_{i} & 0
\end{bmatrix}.\tag{1.6} $$
These follow the anticommutator relation,
$$\{ \gamma^{\mu},\gamma^{\nu} \}=2g^{\mu \nu}.\tag{1.7} $$The $\gamma^{0}$ matrix is Hermitian, $\gamma ^{0\dagger}=\gamma^{0}$, and $(\gamma^{0})^2=\mathbb{I}$. The others are anti-Hermitian $\gamma ^{i\dagger}=-\gamma^{i}$ and $(\gamma^{i})^2=-\mathbb{I}$.
In reality there are Dirac indices in the anticommutator relation $\{ \gamma^{\mu},\gamma^{\nu} \}_{ij}=2g^{\mu \nu}\mathbb{I}_{ij}$ however they are often omitted. The traces are over Dirac indices $ij$ not Lorentz indices $\mu \nu$.

This gives the Dirac equation
$$(i\gamma^{\mu}\partial_{\mu}-m\mathbb{I})_{ij}\psi_{j}=0\tag{1.8} .$$Taking the Hermitian conjugate gives
$$\psi ^{\dagger}\gamma^{0}(i\gamma^{0}\overleftarrow{\partial_{\mu}}+m)=0.\tag{1.9} $$It is convention to write $\psi ^{\dagger}\gamma^{0}=\bar{\psi}$. The arrow over the $\partial_{\mu}$ indicates the direction it acts.

The Lagrangian density is 
$$\mathcal{L}=\bar{\psi}(i\partial \!\!\!/-m)\psi=\bar{\psi}(i\stackrel{\leftrightarrow}{\partial \!\!\!/}-m)\psi \tag{1.10} $$
where
$$\bar{\psi}\stackrel{\leftrightarrow}{\partial \!\!\!/}\psi=\frac{1}{2}\bar{\psi}(\overrightarrow{\partial}\!\!\!/\psi)-\frac{1}{2}(\bar{\psi}\overleftarrow{\partial \!\!\!/})\psi.\tag{1.11} $$
