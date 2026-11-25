To introduce the coupling of the particle into the [[Klein-Gordon Equation]], the [[4-Potential]] is needed,
$$A^{\mu}=\begin{bmatrix}
\frac{\phi}{c} \\
\underline{A}
\end{bmatrix}.$$
For minimal coupling, $E\to E-q\phi$, $\underline{p}\to \underline{p}-q\underline{A}$ or
$$p^{\mu}\to p^{\mu}-qA^{\mu}.$$
Applying minimal coupling and the correspondence principle, $p^{\mu}\to i\hbar \partial^{\mu}$, to the Klein-Gordon equation,
$$p^2\Phi=m^2c^2\Phi$$
$$\therefore (i\hbar \partial^{\mu}-qA^{\mu})(i\hbar \partial_{\mu}-qA_{\mu})\Phi(\underline{x},t)=m^2c^2\Phi(\underline{x},t).$$
In component notation,
$$\left[ \frac{1}{c^2}\left( i\hbar \frac{\partial}{\partial t}-q\phi \right)^2-(-i\hbar \underline{\nabla}-q\underline{A})^2 \right]\Phi(\underline{x},t)=m^2c^2\Phi(\underline{x},t).$$
Take the non-relativistic limit to see if it gives the Schrodinger equation.
$$E=\gamma mc^2=\frac{mc^2}{\sqrt{ 1-\frac{v^2}{c^2} }}\approx mc^2+\frac{1}{2}mv^2+\mathcal{O}(v^4).$$
Take $\tilde{E}=E-mc^2$ which is the non-relativistic kinetic energy. 
Redefine the wavefunction to remove the rest mass energy.
$$\Phi(\underline{x},t)=e^{ -imc^2t/\hbar }\tilde{\Phi}(\underline{x},t)$$
$$\left( i\hbar \frac{\partial}{\partial t}-q\phi \right)\Phi(\underline{x},t)=i\hbar \left( -\frac{imc^2}{\hbar}t \right)\tilde{\Phi}(\underline{x},t)+i\hbar e^{ -imc^2t/\hbar } \frac{\partial\tilde{\Phi}}{\partial t}-q\phi e^{ -imc^2t/\hbar }\tilde{\Phi}(\underline{x},t)$$
$$=e^{-imc^2/\hbar}\left( i\hbar \frac{\partial}{\partial t} +mc^2-q\phi \right)\tilde{\Phi}(\underline{x},t)$$
$$\therefore \left( i\hbar \frac{\partial}{\partial t}-q\phi \right)^2\Phi(\underline{x},t)=e^{ -imc^2t/\hbar }\left( i\hbar \frac{\partial}{\partial t}+mc^2-q\phi \right)^2\tilde{\Phi}(\underline{x},t).$$
Substituting this into the Klein-Gordon equation gives
$$\cancel{e^{ -imc^2t/\hbar }}\left[ \frac{1}{c^2}\left( i\hbar \frac{\partial}{\partial t}+mc^2-q\phi \right)^2-(-i\hbar \underline{\nabla}-q\underline{A})^2 \right]\tilde{\Phi}(\underline{x},t)=mc^2\cancel{e^{-imc^3t/\hbar}}\tilde{\Phi}(\underline{x},t).$$
$$\left[ \left( i\hbar \frac{\partial}{\partial t}+mc^2-q\phi \right)^2-m^2c^4 \right]\tilde{\Phi}(\underline{x},t)=(i\hbar \underline{\nabla}+q\underline{A})^2c^3\tilde{\Phi}(\underline{x},t).$$
Expand the LHS:
$$-\hbar^2 \frac{\partial^2\tilde{\Phi}}{\partial t^2}+i\hbar \frac{\partial}{\partial t}[(mc^2-q\phi)^2\tilde{\Phi}]+(mc^2-q\phi)^2i\hbar \frac{\partial \tilde{\Phi}}{\partial t}-\cancel{m^2c^4}\tilde{\Phi}+(\cancel{m^2c^4}-2mc^2q\phi+q^2ohi^2)\tilde{\Phi}$$
$$=-\hbar^2 \frac{\partial^2\tilde{\Phi}}{\partial t^2}-i\hbar \frac{\partial \phi}{\partial t}\tilde{\Phi}+2(mc^2-q\phi)i\hbar \frac{\partial \tilde{\Phi}}{\partial t}-2mc^2q\phi \tilde{\Phi}+q^2\phi^2\tilde{\Phi}.$$
Assume the wavefunction is slowly evolving and the electromagnetic field is small enough that the non-relativistic approximation is valid:
$$|q\phi|\ll mc^2;\; \left\lvert  \hbar \frac{\partial \phi}{\partial t}  \right\rvert \ll mc^2\phi;\;\left\lvert  \hbar^2 \frac{\partial^2\tilde{\Phi}}{\partial t^2}  \right\rvert\ll \left\lvert  mc^2 \frac{\partial \tilde{\Phi}}{\partial t}  \right\rvert. $$
This leaves
$$2mc^2i\hbar \frac{\partial \tilde{\Phi}}{\partial t}-2mc^2q\phi \tilde{\Phi}.$$
$$\implies 2mc^2\left[ i\hbar \frac{\partial \tilde{\Phi}}{\partial t}-q\phi \tilde{\Phi} \right]=(i\hbar \underline{\nabla}+q\underline{A})^2c^2\tilde{\Phi}.$$
$$\implies i\hbar \frac{\partial \tilde{\Phi}}{\partial t}=\left[ \frac{1}{2m}(i\hbar \underline{\nabla}+q\underline{A})^2+q\phi \right]\tilde{\Phi}.$$
This is the [Schrodinger equation](Hamiltonian%20for%20Particles%20in%20EM%20field.md) for a particle in an electromagnetic field.
