We can [choose](Gauge%20Transformations.md) a $\lambda'$ s.t. $\underline{\nabla}\cdot \underline{A}'=0$:
$$\underline{\nabla}\cdot \underline{A}'=\underline{\nabla}\cdot(\underline{A}+\underline{\nabla}\lambda)=\underline{\nabla}\cdot \underline{A}+\nabla^2\lambda.$$
$$\implies \nabla^2\lambda=-\underline{\nabla}\cdot \underline{A}.$$
From this the scalar field in the Coulomb gauge,
$$\nabla^2\phi=\frac{\rho}{\varepsilon_{0}}.$$
This is known as the Poisson equation. By setting $\lim_{ r \to \infty }\phi(\underline{r})=0$, we have the solution
$$\phi(\underline{r},t)=\frac{1}{4\pi \varepsilon_{0}}\int \frac{\rho(\underline{r}',t)}{\lvert \underline{r}-\underline{r}' \rvert }dr'$$
![[Pasted image 20241102081437.png]]
The vector potential is more difficult to calculate in this gauge, and can be found by solving the equation
$$\nabla^2\underline{A}-\mu_{0}\varepsilon_{0} \frac{\partial^2\underline{A}}{\partial t^2}=\mu_{0}\underline{j}+\mu_{0}\varepsilon_{0}\underline{\nabla}\left( \frac{\partial \phi}{\partial t} \right).$$
