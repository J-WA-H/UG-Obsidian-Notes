For quantum dynamics, we need to consider the different pictures of quantum mechanics.

The Schrodinger picture is described by a wavefunction $\ket{\psi}$ which obeys the Schrodinger equation
$$\tag{1.1} i\hbar \frac{d\ket{\psi}}{dt}=\hat{H}\ket{\psi}.$$For a time-independent Hamiltonian $\hat{H}$, the solution to this is
$$\ket{\psi(t)} =e^{ -i\hat{H}t/\hbar }\ket{\psi(0)} \tag{1.2} $$
where the exponential describes the time-evolution of the wavefunction.

The Heisenberg picture is described by an operator $\hat{A}$ with no explicit time dependence and obeys the Heisenberg equation
$$\frac{d\hat{A}}{dt}=-\frac{i}{\hbar}[\hat{A},\hat{H}]\tag{1.3}. $$
For a time independent $\hat{H}$, this is solved by
$$\hat{A}(t)=e^{ i\hat{H}t/\hbar }\hat{A}(0)e^{ -i\hat{H}t/\hbar }\tag{1.4} $$which shows the time evolution within the operator.

Although these are two different pictures of quantum mechanics, they both yield the same expectation values.
Consider the expectation value in the Schrodinger picture,
$$
\langle \hat{A}(t) \rangle =\bra{\psi(t)} \hat{A}(0)\ket{\psi(t)}=\bra{\psi(0)} e^{ i\hat{H}t/\hbar }\hat{A}(0)e^{ -i\hat{H}t/\hbar }\ket{\psi(0)} =\bra{\psi(0)} \hat{A}(t)\ket{\psi(0)}   
\tag{1.5} \;\square$$
Consider a quantum mechanical system completely described by $\ket{\psi}$, the [[Density Operator]] is given by
$$\rho=\ket{\psi} \bra{\psi}\tag{1.6}  $$with the implicit tensor product $\ket{\psi}\bra{\psi}=\ket{\psi}\otimes \bra{\psi}$. Note that for some density operator $\rho$, the same $\rho$ derives from the wavefunction $e^{ i\phi }\ket{\psi}$, $(e^{ i\phi }\ket{\psi})(e^{ -i\phi }\bra{\psi})=\ket{\psi}\bra{\psi}=\rho$. This shows that global phase has no measurable so is not needed.

The density operator can be used to derive the [[Von-Neumann Equation]] from the time-dependent Schrodinger equation,
$$i\hbar \frac{d\rho}{dt}=i\hbar \frac{d\ket{\psi}}{dt}\bra{\psi} +i\hbar \ket{\psi} \frac{d\bra{\psi}}{dt}=[\hat{H},\ket{\psi} \bra{\psi} ].\tag{1.7}     $$This yields the Von-Neumann equation
$$\frac{d\rho}{dt}=-\frac{i}{\hbar}[\hat{H},\rho].\tag{1.8} $$
From this expectation values are determined by the trace,
$$\langle \hat{A}(t) \rangle =\mathrm{Tr}(\rho(t)\hat{A}(0))=\mathrm{Tr}(\rho(0)\hat{A}(t)).\tag{1.9} $$
If $\rho=\ket{\psi}\bra{\psi}$, from the cyclic property of the trace,
$$\langle \hat{A}(t) \rangle =\mathrm{Tr}(\ket{\psi(t)} \bra{\psi(t)} \hat{A}(0))=\mathrm{Tr}(\bra{\psi(t)} \hat{A}(0)\ket{\psi(t)} )=\bra{\psi(t)} \hat{A}(t)\ket{\psi(t)} \;\square \tag{1.10}  $$

There are also different pictures to describe classical dynamics.

Consider a 1D classical particle with coordinate $x$, momentum $p$ and Hamiltonian $H$. Hamilton's equation of motion for some function $A(x,p)$ are given in terms of a Poisson bracket,
$$\frac{dA}{dt}=\{ A,H \}=\frac{\partial A}{\partial x} {\frac{\partial H}{\partial p}}-\frac{{\partial A}}{\partial p} \frac{{\partial H}}{\partial x}.\tag{1.11} $$This is the classical limit of the Heisenberg equations.

The Liouville equation describes the dynamics of phase space distribution (the joint probability distribution of coordinates and momentum) $\rho_{PS}(x,p)$,
$$\frac{\partial \rho_{PS}}{\partial t}=\{ H,\rho_{PS} \}=\frac{{\partial H}}{\partial x} \frac{{\partial \rho_{PS}}}{\partial p}-\frac{{\partial H}}{\partial p} \frac{{\partial \rho_{PS}}}{\partial x}.\tag{1.12} $$This is the classical limit of the Von-Neumann equation.

In the Hamilton picture, the classical expectation value is given by the distribution of initial values $\rho_{PS}(0)=\rho_{PS}(x_{0},p_{0})$
$$\langle A(t) \rangle =\iint dx_{0}dp_{0}A(x_{0},p_{0},t)\rho_{PS}(x_{0},p_{0})\tag{1.13} $$while in the Liouville picture,
$$\langle A(t) \rangle =\iint dxdpA(x,p)\rho_{PS}(x,p,t).\tag{1.14} $$
Example: Gaussian initial distribution
Consider the double Gaussian of initial positions and momenta:
$$\rho_{PS}(x_{0},p_{0})=\frac{1}{2\pi\sigma_{x}\sigma_{p}}\exp\left[ -\frac{(x_{0}-\mu_{x})^2}{2\sigma_{x}^2} -\frac{(p_{0}-\mu_{p})^2}{2\sigma_{p}^2}\right].\tag{1.15} $$
So the expectation value in the Hamilton picture is
$$\langle x(t) \rangle =\frac{1}{2\pi\sigma_{x}\sigma_{p}}\iint dx_{0}dp_{0}\exp\left[-\frac{(x_{0}-\mu_{x})^2}{2\sigma_{x}^2} -\frac{(p_{0}-\mu_{p})^2}{2\sigma_{p}^2}\right]\tag{1.16}. $$
For free particles, $x(x_{0},p_{0}.t)=x+p_{0} \frac{t}{m}$ so
$$\langle x(t) \rangle =\frac{1}{\sqrt{ 2\pi\sigma_{x}^2 }}\int dx_{0}x_{0}\exp\left[ -\frac{(x_{0}-\mu_{x})^2}{2\sigma_{x}^2} \right]+\frac{1}{\sqrt{ 2\pi\sigma_{p}^2 }}\int dp_{0} \frac{p_{0}t}{m}\exp\left[ -\frac{(p_{0}-\mu_{p})^2}{2\sigma_{p}^2} \right]\tag{1.17} $$
which, when evaluated, gives
$$\langle x(t) \rangle =\mu_{x}+\frac{\mu_{p}t}{m}.\tag{1.18} $$
Note that $p(t)=p_{0}$, $x_{0}=x(t)-p(t)t/m$ and $dx_{0}dp_{0}=dx(t)dp(t)$, hence
$$\langle x(t) \rangle =\frac{1}{2\pi\sigma_{x}\sigma_{p}}\iint dx(t)dp(t)x(t)\exp\left[ -\frac{(x(t)-p(t)t/m-\mu_{x})^2}{2\sigma_{x}^2}-\frac{(p(t)-\mu_{p})^2}{2\sigma_{p}^2} \right]=\iint dxdpx\rho_{PS}(x,p,t).\tag{1.19} $$
The Wigner function is an attempt at something like a joint position and momentum distribution for a quantum mechanical particle,
$$W(x,p)=\frac{1}{2\pi \hbar}\int d\xi \bra{x+\frac{\xi}{2}} p\ket{x-\frac{\xi}{2}} \exp\left[ -\frac{i\xi p}{\hbar} \right].\tag{1.20}  $$From this a symmetrised expectation value can be determined,
$$\iint dxdpxpW(x,p)=\frac{{\langle \hat{x}\hat{p}+\hat{p}\hat{x} \rangle}}{2}. \tag{1.21} $$Unlike probability distributions, the Wigner function can take negative values.

Two time correlation functions generalise single time expectation values. They effectively require the Heisenberg of Hamilton picture formulation.

The quantum example is
$$\langle \hat{x}(t)\hat{x}(t') \rangle =\mathrm{Tr}(\rho(0)\hat{x}(t)\hat{x}(t'))\tag{1.22} $$
while the classical equivalent is
$$\langle x(t)x(t') \rangle =\iint dx_{0}dp_{0}x(x_{0},p_{0},t)x(x_{0},p_{0},t')\rho_{PS}(x_{0},p_{0}).\tag{1.23} $$
