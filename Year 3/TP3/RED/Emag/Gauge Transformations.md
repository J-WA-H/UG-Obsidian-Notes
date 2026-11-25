A gauge transformation is a modification to the [potentials](Vector%20and%20Scalar%20Potentials.md) that leave $\underline{E}$ and $\underline{B}$ invariant.
$$\underline{A}'(\underline{r},t)=\underline{A}(\underline{r},t)+\underline{\alpha}(\underline{r},t)$$
$$\phi'(\underline{r},t)=\phi(\underline{r},t)+\beta(\underline{r},t)$$
To leave $\underline{B}$ invariant we need $\underline{\nabla}\times \underline{A}=\underline{\nabla}\times \underline{A}'=\underline{\nabla}\times(\underline{A}+\underline{\alpha})\implies \underline{\nabla}\times \underline{\alpha}=\underline{0}$.
This condition on $\underline{\alpha}$ is satisfied if it it can be written as the grad of some scalar $\lambda$
$$\underline{\alpha}=\underline{\nabla}\lambda.$$
To leave $\underline{E}$ invariant, 
$$-\underline{\nabla}\phi-\frac{\partial \underline{A}}{\partial t}=-\underline{\nabla} \phi'-\frac{\partial \underline{A}'}{\partial t}=-\underline{\nabla}\phi-\frac{\partial \underline{A}}{\partial t}-\left( \underline{\nabla}\beta +\frac{\partial\underline{\alpha}}{\partial t} \right)$$
$$\implies \underline{\nabla}\beta+\frac{\partial \underline{\alpha}}{\partial t}=\underline{0}.$$
Using $\underline{\alpha}=\underline{\nabla}\lambda$ we have
$$\underline{\nabla}\left( \beta+\frac{\partial \lambda}{\partial t} \right)=\underline{0}.$$
As this grad is zero, $\beta+\frac{\partial \lambda}{\partial t}$ is independent of space. 
Lets call
$$\kappa(t)=\beta(\underline{r},t)+\frac{\partial \lambda(\underline{r},t)}{\partial t}.$$
Take the integral over time
$$\int \kappa(t')dt'=\int\left[ \beta(\underline{r},t')+\frac{\partial \lambda}{\partial t'} \right]dt'=\lambda+\int \beta(\underline{r},t')dt'.$$
We can define $\lambda'$ as
$$\lambda'=\lambda-\int_{0}^t\kappa(t')dt'.$$
$$\underline{\nabla}\lambda'=\underline{\nabla}\lambda+\underline{\nabla}\cancelto{0}{\left( \int_{0}^t\kappa(t')dt' \right)}=\underline{\alpha}.$$
The $\kappa$ term cancels as by definition it is independent of position.

Take time derivative of $\lambda$:
$$\frac{\partial \lambda'}{\partial t}=\frac{\partial \lambda}{\partial t}-\frac{\partial}{\partial t}\left( \int_{0}^t\kappa(t)dt \right)=\frac{\partial \lambda}{\partial t}-\kappa(t)=\frac{\partial \lambda}{\partial t}-\beta-\frac{\partial \lambda}{\partial t}=-\beta.$$
As we have found relations for $\underline{\alpha}$, $\beta$ in terms of $\lambda'$ so we can write the gauge transformation as:
$$\underline{A}'=\underline{A}+\underline{\nabla}\lambda'$$
$$\phi'=\phi-\frac{\partial \lambda'}{\partial t}.$$
