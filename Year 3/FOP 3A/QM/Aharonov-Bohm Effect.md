Consider a particle moving along a ring of fixed radius $\rho=b$.
![[Pasted image 20241019123422.png]]
To calculate the energy levels, cylindrical coordinates will be used. There is no potential as the B filed is zero so
$$\hat{H}=-\frac{\hbar^2}{2m}\nabla^2$$
In cylindrical coords, $$\nabla^2=\frac{1}{\rho} \frac{\partial}{\partial \rho}\left( \rho      \frac{\partial}{\partial \rho} \right)+\frac{1}{\rho^2} \frac{\partial^2}{\partial \phi^2}+\frac{\partial^2}{\partial z^2}.$$
As the motion of the particle is constrained to a circle in the x,y plane of constant radius,
$$\frac{\partial}{\partial z}=\frac{\partial}{\partial \rho}=0.$$
so$$\hat{H}\psi=-\frac{\hbar^2}{2m} \frac{1}{\rho^2} \frac{\partial^2\psi}{\partial \phi^2}=E\psi.$$
Take $\psi(\phi)=\frac{e^{in\phi}}{\sqrt{ 2\pi }}$ as there is no potential confining the particle in space. This gives an energy of
$$E_{n}=\frac{\hbar^2n^2}{2mb^2}$$
where $n\in \mathbb{Z}$.

Now add a solenoid where inside $\underline{B}=B\hat{\underline{z}}$, and outside $\underline{B}=\underline{0}$.
![[Pasted image 20241019123336.png]]
We can now use the [Hamiltonian](Hamiltonian%20for%20Particles%20in%20EM%20field.md) in an EM field, choosing the gauge
$$\underline{A}=A_{\phi}(\rho)\underline{\hat{\phi}}\text{ and }\phi=0$$
where
$$A_{\phi}(\rho)=\begin{cases}
\frac{B\rho}{2} & \rho<a \\
\frac{Ba}{2\rho} & \rho>a
\end{cases}.$$
$$\hat{H}=\frac{1}{2m}(-i\hbar \underline{\nabla}-q\underline{A})^2$$
$$\hat{H}=\frac{1}{2m}\left( -\frac{i\hbar}{\rho}\underline{\hat{\phi}} \frac{\partial}{\partial \phi}-\frac{q\Phi_{B}}{2\pi \rho} \right)^2=\frac{\hbar^2}{2mb^2}\left( -\frac{\partial^2}{\partial \phi^2}+\frac{2iq\Phi_{B}}{h} \frac{\partial}{\partial \phi}+\left( \frac{q\Phi_{B}}{h} \right)^2 \right)$$
$$\implies \frac{\hbar^2}{2mb^2}\left[ -\frac{\partial^2}{\partial \phi^2}+\frac{2iq\Phi_{B}}{h} \frac{\partial}{\partial \phi}+\left( \frac{q\Phi_{B}}{h} \right)^2 \right]\psi(\phi)=E\psi(\phi).$$
Again as there is no potential confining the particle, take $\psi(\phi)=e^{in\phi}$ which gives energy levels
$$E_{n}=\frac{\hbar^2}{2mb^2}\left[ n-\frac{\Phi_{B}}{\left( \frac{h}{q} \right)} \right]^2$$
