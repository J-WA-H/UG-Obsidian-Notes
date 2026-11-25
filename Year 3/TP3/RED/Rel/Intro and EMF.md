Maxwell's equations describe the nature of electromagnetic fields.
$$\underline{\nabla} \cdot \underline{E} = \frac{\rho}{\varepsilon_{0}}$$
$$\underline{\nabla} \cdot \underline{B} = 0$$
$$\underline{\nabla} \times \underline{E} = - \frac{\partial\underline{B}}{\partial t}$$
$$\underline{\nabla} \times \underline{B} = \mu_{0} \underline{j} + \varepsilon_{0} \mu_{0} \frac{{\partial \underline{E}}}{\partial t}.$$

Another important equation that describes electromagnetic fields is the Lorentz force - the force experienced by a charged particle moving in electric and magnetic fields
$$\underline{F}=q(\underline{E}+\underline{v}\times \underline{B}).$$
Maxwell's equations can be used to derive a wave equation for EM waves which gives a speed of
$$c=\frac{1}{\sqrt{\varepsilon_{0} \mu_{0}}}.$$
![[20241007_191028.jpg]]

Consider the following cases in the above diagram
1. S is at rest with respect to $\underline{B}$:
	As there is no electric field, the force experienced by the charge is given by $\underline{F} =q(\underline{v}\times \underline{B})$.
2. S' at rest with respect to the charge:
	As the particle is at rest in this frame, $\underline{v}=\underline{0}$, so $\underline{F}=\underline{0}$, implying that the particle is either at rest or moving in a straight line w.r.t the magnetic field - contradicting the force given in the S frame.
	Maxwell's equations solve this. As, in the S' frame, the $\underline{B}$ field is moving relative to the charge so $\frac{{\partial \underline{B}}}{\partial t}\neq 0$. Using Maxwell III, this gives $\underline{\nabla}\times \underline{E} \neq 0$ so there is an $\underline{E}$ field generating by this moving $\underline{B}$ field, yielding a force $\underline{F}=q\underline{E}$, fixing this paradox.
This shows that even though the two frames disagree on which field generates this force, they both agree that the particle experiences a force that is equivalent to each other.

![[Pasted image 20241007203326.png]]
The above figure shows a current loop with a magnet moving towards it at speed $\underline{v}_{M}$.
In the rest frame of the wire loop, the magnet is moving towards it, so using Maxwell III there is an $\underline{E}$ field. The force is given by $\underline{F}=q\underline{E}.$ The electromotive force of this system is given by
$$\varepsilon = \oint_{C} \frac{{\underline{F}}}{q}\cdot d\underline{l}=\oint_{C}\underline{E}\cdot d\underline{l}$$
$$=\oint_{S}(\underline{\nabla}\times \underline{E})\cdot d\underline{A}=-\frac{\partial}{\partial t}\oint_{S}\underline{B}\cdot d\underline{A}$$
$$\implies \varepsilon=-\frac{{\partial \Phi}}{\partial t}\text{   Faraday's law.}$$
To check this also works in the rest frame of the magnet, where the wire is moving towards the magnet at speed $\underline{v}_{c}$.
Consider the fractional change in magnetic flux:
$$\delta \Phi =\int_{S(t+\delta t)}\underline{B}(t+\delta t)\cdot d\underline{A}-\int_{S(t)}\underline{B}(t)\cdot d\underline{A}$$
Take the Taylor expansion of $\underline{B}(t+\delta t)$:
$$\underline{B}(t+\delta t)= \underline{B}(t)+\frac{\partial}{\partial t}\underline{B}(t)|_{\delta t}.$$
$$\therefore \delta \Phi=\int_{S(t+\delta t)} \frac{\partial\underline{B}(t)}{\partial t}\cdot d\underline{A}\delta t+\int_{S(t+\delta t)}\underline{B}(t)\cdot d\underline{A}-\int_{S(t)}\underline{B}(t)\cdot d\underline{A}$$
Use divergence theorem to show the far right term is zero:
$$\int_{S(t)}\underline{B}.d\underline{A}=\int_{V}\underline{\nabla}\cdot \underline{B}\;dV=0$$
Calculate area element:
$$d\underline{A}=d\underline{l}\times \underline{v}\delta t \implies \underline{B}\cdot d\underline{A}=\underline{B}\cdot(d\underline{l}\times \underline{v})\delta t =-d\underline{l}\cdot(\underline{v}\times \underline{B})\delta t.$$
$$\int_{S(t+\delta t)} \frac{\partial\underline{B}}{\partial t}\cdot d\underline{A}=-\int(\underline{\nabla}\times \underline{E})\cdot d\underline{A}=-\int \underline{E}\cdot d\underline{l}$$
$$\therefore \delta \Phi=-\int dl\cdot(\underline{v}\times \underline{B})\delta t-\int \underline{E}\cdot d\underline{l}\delta t$$
$$\implies \delta \Phi=-\int(\underline{E}+\underline{v}\times \underline{B})\cdot d\underline{l}\delta t=-\int \frac{\underline{F}}{q}\cdot d\underline{l}\delta t$$
Take limits as $\delta \Phi \rightarrow{0}$ and $\delta t\rightarrow 0$:
$$\frac{\partial\Phi}{\partial t}=-\int \frac{\underline{F}}{q}\cdot d\underline{l}=-\varepsilon$$
Faraday's law holds in both reference frames.