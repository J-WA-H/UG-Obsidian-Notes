For two identical non-interacting particles with wavefunctions $\phi_{1},\phi_{2}$, it holds that
$$\braket{ \phi_{1} | \phi_{2} } =\int d^3r\phi_{1}^{*}(\vec{r})\phi_{2}(\vec{r})=0\tag{1.1} .$$
For indistinguishable particles, the wavefunctions are superpositions of the products of $\phi_{1},\phi_{2}$ that obey the correct symmetry,
$$\begin{matrix}
\psi_{s}(\vec{r},\vec{r}')=\frac{1}{\sqrt{ 2 }}[\phi_{1}(\vec{r})\phi_{2}(\vec{r}')+\phi_{2}(\vec{r})\phi_{1}(\vec{r}')] & \text{symmetric} \\
\psi_{a}(\vec{r},\vec{r}') = \frac{1}{\sqrt{ 2 }} [\phi_{1}(\vec{r})\phi_{2}(\vec{r}')-\phi_{2}(\vec{r})\phi_{1}(\vec{r}')] & \text{antisymmetric}
\end{matrix}\tag{1.2}. $$
If particles are distinguishable, then they are described by a simple product wavefunction
$$\begin{matrix}
\psi^{dis}(\vec{r},\vec{r}')=\phi_{1}(\vec{r})\phi_{2}(\vec{r}') & \text{or} & \psi^{dis}(\vec{r},\vec{r}')=\phi_{1}(\vec{r}')\phi_{2}(\vec{r})
\end{matrix}.\tag{1.3} $$
If $\psi$ is a normalised state in the Hilbert space of states that describe systems of particles, the Hamiltonian operator of the system is $H$ and 
$$H\psi_{n}=E_{n}\psi_{n}\tag{1.4} .$$The [[Rayleigh-Ritz Variational Principle]] for a normalised state gives
$$\bra{\psi} H\ket{\psi} \geq E_{0}\tag{1.5}  .$$
The method of [[Lagrange Multipliers]] allows us to maximise $f(x_{1},x_{2},\dots,x_{n})$ with the constraint $g(x_{1},x_{2},\dots,x_{n})=c$. This method maximises
$$f(x_{1},x_{2},\dots,x_{n})+\lambda g(x_{1},x_{2},\dots,x_{n})\tag{1.6} .$$
To do this solve for
$$\frac{\partial}{\partial x_{i}}(f+\lambda g)=0\tag{1.7} .$$
This gives solutions of the form $x_{i}=x_{i}(\lambda)$. $\exists$ $\lambda_{0}$ s.t. $g(x_{1}(\lambda_{0}),x_{2}(\lambda_{0}),\dots,x_{n}(\lambda_{0}))=c$ and $f(x_{1}(\lambda_{0}),x_{2}(\lambda_{0}),\dots,x_{n}(\lambda_{0}))$ is maximised with the constraint.

Consider that the total energy is defined by [[Functionals]] dependent on the wavefunction $E[\phi]=\bra{\phi}h\ket{\phi}$. The functional derivative is the derivative of $E$ when we vary the wavefunction $\phi\to \phi+\varepsilon u$.
$$\frac{\delta E}{\delta\phi}=\lim_{ \varepsilon \to 0 } \frac{{E[\phi+\varepsilon u]-E[\phi]}}{\varepsilon}. \tag{1.8}  $$
When $E$ is minimised with respect to $\phi$, this derivative must vanish $\forall$ $u$. The minimisation is constrained by $\braket{ \phi | \phi }=1$ so we instead minimise $$G[\phi]=E[\phi]-\lambda \braket{ \phi | \phi } =\bra{\phi} h\ket{\phi} -\lambda \braket{ \phi | \phi }\tag{1.9}  $$$$\therefore \lim_{ \varepsilon \to 0 } \frac{{G[\phi+\varepsilon u]-G[\phi]}}{\varepsilon}=\lim_{ \varepsilon \to 0 } \frac{{(\bra{\phi+\varepsilon u} h\ket{\phi+\varepsilon u} -\lambda \braket{ \phi+\varepsilon u | \phi+\varepsilon u } )-(\bra{\phi} h\ket{\phi} -\lambda \braket{ \phi | \phi } )}}{\varepsilon}=0.\tag{1.10}$$
