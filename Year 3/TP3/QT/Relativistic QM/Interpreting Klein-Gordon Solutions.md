The [[Klein-Gordon Equation]] behaves as expected - it is Lorentz invariant and the low energy limit gives the Schrodinger equation.

The aim is to derive a continuity equation such that
$$\underline{\nabla}\cdot \underline{j}=\frac{\partial\rho}{\partial t}$$
where $\underline{j}$ is the probability current and $\rho$ is the probability density.
$$\rho=\Phi^{*} \frac{\partial \Phi}{\partial t}-\Phi  \frac{\partial \Phi^{*}}{\partial t}$$
$$\underline{j}=\Phi \underline{\nabla}\Phi^{*}-\Phi^{*}\underline{\nabla}\Phi.$$
We want this to reduce to the Schrodinger equation in the non-relativistic limit. This suggests that we have the relativistic analogue of the conservation of probability current.

This is not straight forward as $\rho$ is not necessarily positive so we can have a negative probability density - which is unphysical.
This lead to doubts about the consistency of the Klein-Gordon equation as a relativistic quantum theory.

Another problem comes about if we consider solutions to the free Klein-Gordon equation,
$$\Phi(\underline{x},t)=Ae^{ i(\underline{k}\cdot \underline{x}-\omega t) }.$$
We can write $k$ as a 4-vector,
$$k^{\mu}=\begin{bmatrix}
\frac{\omega}{c} \\
\underline{k}
\end{bmatrix}.$$
$$\therefore i(\underline{k}\cdot \underline{r}-\omega t)=-ik^{\mu}x_{\mu}.$$
Plug this solution into the Klein-Gordon equation.
$$\left( \frac{1}{c^2} \frac{\partial^2}{\partial t^2} -\nabla^2+\frac{m^2c^2}{\hbar^2}\right)\Phi(\underline{x},t)=0$$
$$\implies \omega^2-k^2c^2=\frac{m^2c^2}{\hbar^2}$$
$$\omega=\pm \sqrt{ k^2c^2+\frac{m^2c^2}{\hbar^2} }.$$
Since energy is $\hbar \omega$, this gives negative energy solutions, which is another problem

This led to the Klein-Gordon equation being largely discarded.

This interpretation can be solved in quantum field theory. The Klein-Gordon equation describes spin 0 particles. The positive energy corresponds to the particle and negative energy corresponds to the antiparticle.
