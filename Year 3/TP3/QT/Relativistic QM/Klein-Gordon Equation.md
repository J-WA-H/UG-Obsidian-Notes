So far all systems have been described by the Schrodinger equation,
$$H\psi=\left( -\frac{\hbar^2}{2m}\nabla^2+V(r) \right)\psi=i\hbar \frac{\partial \psi}{\partial t}.$$
This can be obtained using the correspondence principle - a quantum mechanical analogue of classical equations.

First find the classical equation for the Hamiltonian then replace classical observables with quantum operators,
$$E\to i\hbar \frac{\partial}{\partial t};\;\underline{p}\to-i\hbar \underline{\nabla}.$$
For the Schrodinger equation;
$$H=T+V=\frac{1}{2}mv^2+V(r)=\frac{p^2}{2m}+V(r)$$
Swapping out observables gives
$$H\psi=\left[ -\frac{\hbar^2}{2m}\nabla^2+V(r) \right]\psi=E\psi=i\hbar \frac{\partial \psi}{\partial t}.$$
This is first quantisation.

Now consider relativistic [energy/momentum](4-Momentum.md):
$$E^2=p^2c^2+m^2c^4.$$
Using correspondence principal
$$E^2\to-\hbar^2 \frac{\partial^2}{\partial t^2};\; p^2\to-\hbar^2\nabla^2$$
$$\therefore -\hbar^2 \frac{\partial^2\Phi}{\partial t^2}=(-\hbar^2c^2\nabla^2+m^2c^4)\Phi.$$
This is the Klein-Gordon equation.

This can be simplified using [tensor notation](Relativistic%20Wave%20Equations.md),
$$\begin{bmatrix}
\frac{E}{c} \\
\underline{p}
\end{bmatrix}\to \begin{bmatrix}
\frac{i\hbar}{c} \frac{\partial}{\partial t} \\
-i\hbar \underline{\nabla}
\end{bmatrix}=-i\hbar \partial^\mu$$
$$p^{\mu}\to-i\hbar \partial^{\mu}$$
Considering the norm of $p^{\mu}$,
$$p^2=m^2c^2$$
$$-\hbar^2\partial^{\mu}\partial_{\mu}\Phi(\underline{x},t)=m^2c^2\Phi(\underline{x},t)$$
i.e.
$$\left( \partial^{\mu}\partial_{\mu}+\frac{m^2c^2}{\hbar^2} \right)\Phi(\underline{x},t)=0.$$
Note unlike the Schrodinger equation, this has both time and space derivatives being of second order. This equation is Lorentz invariant.

In natural units,
$$(\partial^{\mu}\partial_{\mu}+m^2)\Phi(\underline{x},t)=0.$$
