When an external B-field is applied to a superconductor, a [supercurrent](Superconductivity.md) is generated.
This induces a B-field which cancels the applied B-field which causes the superconductor to levitate. This is the Meissner effect.

This can be described by the London equation,
$$\underline{j}=-\frac{1}{\mu_{0}\lambda_{L}^2}\underline{A}$$
where $\underline{A}$ is a [vector potential](Vector%20and%20Scalar%20Potentials.md) and $\lambda_{L}$ is the London penetration depth.

As we are using a vector potential, we need to define a gauge. Here the London gauge will be used - $\underline{\nabla}\cdot \underline{A}=0$.
This implies that $\underline{\nabla}\cdot \underline{j}=0$, which shows charge conservation.
Proof:
Consider an infinitesimal cube of side length $\Delta x$
![[Pasted image 20250227111920.png]]
By definition the rate of change of the carrier concentration is proportional to the difference in current at two opposite faces,
$$\frac{ \partial n }{ \partial t } \propto[j(x+\Delta x)-j(x)]\propto \frac{dj}{dx}.$$
Moving to 3D,
$$\frac{ \partial n }{ \partial t } \propto \underline{\nabla}\cdot \underline{j}.$$
As $\underline{\nabla}\cdot \underline{j}=0$, this implies the carrier concentration doesn't change over time - so charge is conserved $\square$

Consider the curl of the London equation,
$$\underline{\nabla}\times \underline{j}=-\frac{1}{\mu_{0}\lambda_{L}^2}\underline{\nabla}\times \underline{A}=-\frac{\underline{B}}{\mu_{0}\lambda_{L}^2}.$$
Considering Maxwell IV:
$$\underline{\nabla}\times \underline{B}=\mu_{0}\underline{j},$$
$$\underline{\nabla}\times \underline{\nabla}\times \underline{B}=-\frac{\underline{B}}{\lambda_{L}^2}$$
Using the identity
$$\underline{\nabla} \times \underline{\nabla}\times \underline{B}=\underline{\nabla}(\underline{\nabla}\cdot \underline{B})-\nabla^2\underline{B}$$
and Maxwell II $\underline{\nabla}\cdot \underline{B}=0$,
$$\nabla^2\underline{B}=\frac{\underline{B}}{\lambda_{L}^2}.$$
Consider the component along the $z$ axis,
$$\left( \frac{\partial^2}{\partial x^2}+\frac{\partial^2}{\partial y^2}+\frac{\partial^2}{\partial z^2} \right)B_{z}(\underline{r})=\frac{B_{z}(\underline{r})}{\lambda_{L}^2}.$$
Apply this to a semi-infinite slab
![[Pasted image 20250227113428.png]]
The solid is infinite in the $yz$ plane and the $+x$ axis. Apply a uniform B-field, $B_{a}$, along the $z$ axis.
To maintain continuity, we would expect the B-field to have the same magnitude at $x\leq 0$ but will slowly decays as $x> 0$.
As it is infinite in the $yz$ plane, $B_a$ is only dependent on $x$ so
$$\frac{d^2B_{z}}{dx^2}=\frac{B_{z}}{\lambda_{L}^2}$$
$$\implies B_{z}(x)=Ae^{x/\lambda_{L}}+Be^{-x/\lambda_{L}}.$$Since the B-field must decay to zero, assuming perfect [[Diamagnetism]], we impose the boundary condition
$$\lim_{ x \to \infty } B_{z}(z)=0$$
which imposes $A=0$,
$$B_{z}(x)=Be^{-x/\lambda_{L}}.$$
The second boundary condition is from continuity, $B_{z}(0)=B_{a}$
$$\therefore B_{z}(x)=B_{a}e^{-x/\lambda_{L}}.$$
Plotting this gives
![[Pasted image 20250227114323.png]]
This B-field can be used to find the supercurrent,
$$\mu_{0}\underline{j}=\underline{\nabla}\times \underline{B}=\begin{bmatrix}
\frac{\partial}{\partial x} \\
\frac{\partial}{\partial y} \\
\frac{\partial}{\partial z}
\end{bmatrix}\times \begin{bmatrix}
0 \\
0 \\
B_{z}
\end{bmatrix}=\begin{bmatrix}
\cancelto{0}{\frac{ \partial B_{z} }{ \partial y } } \\
-\frac{ \partial B_{z} }{ \partial x }  \\
0
\end{bmatrix}.$$
$$\therefore \underline{j}(x)=-\frac{1}{\mu_{0}} \frac{dB_{z}}{dx}\underline{\hat{y}}=\frac{B_{a}}{\mu_{0}\lambda_{L}}e^{-x/\lambda_{L}}\hat{\underline{y}}.$$

