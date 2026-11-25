Gauge freedom is the fact that different vector potentials can give the same $\underline{B}$ field.
Example:
Take $\phi=0$, $\underline{A}=\frac{B}{2}(\underline{\hat{z}}\times \underline{r})=\frac{B}{2}(-y\underline{\hat{x}}+x\hat{\underline{y}})$
$$\underline{B}=\underline{\nabla}\times \underline{A}=\frac{B}{2}\begin{bmatrix}
\frac{\partial}{\partial x} \\
\frac{\partial}{\partial y} \\
\frac{\partial}{\partial z}
\end{bmatrix}\times \begin{bmatrix}
-y \\
x \\
0
\end{bmatrix}=\frac{B}{2}\begin{bmatrix}
0 \\
0 \\
2
\end{bmatrix}=B\underline{\hat{z}}.$$
Now take $A=-by\underline{\hat{x}}$ (Landau Gauge):
$$\underline{B}=\underline{\nabla}\times \underline{A}=\begin{bmatrix}
\frac{\partial}{\partial x} \\
\frac{\partial}{\partial y} \\
\frac{\partial}{\partial z}
\end{bmatrix}\times \begin{bmatrix}
-By \\
0 \\
0
\end{bmatrix}=B\underline{\hat{z}}.$$
These two different vector potentials give the same B field, which shows that physical observables are the same for each gauge.

Take difference in these gauges:
$$\underline{A}-\underline{A}'=-By\underline{\hat{x}}-\frac{B}{2}(-y\underline{\hat{x}}+x\hat{\underline{y}})=-\frac{B}{2}(y\underline{\hat{x}}-x\hat{\underline{y}})=\underline{\nabla}\left( -\frac{B}{2}xy \right).$$
We define the scalar function inside of the grad operator $\Lambda(\underline{r})$.
$$\underline{A'}(\underline{r})=\underline{A}(\underline{r})+\underline{\nabla}\Lambda(\underline{r}).$$
$$\underline{B}=\underline{\nabla}\times \underline{A}'=\underline{\nabla}\times \underline{A}+\underline{\nabla}\times(\underline{\nabla}\Lambda)$$
As the curl of a grad is zero:
$$\underline{\nabla}\times \underline{A}'=\underline{\nabla}\times \underline{A}.$$
We can use this fact to relate two pairs of gauges that yield the same E and B fields - invariant under a gauge transformation
$$\phi'(\underline{r},t)=\phi(\underline{r},t)-\frac{\partial \Lambda(\underline{r},t)}{\partial t}+c_{1}$$
$$\underline{A}'(\underline{r},t)=\underline{A}(\underline{r},t)+\underline{\nabla}\Lambda(\underline{r},t)+c_{2}.$$
Looking at the [Hamiltonian](Hamiltonian%20for%20Particles%20in%20EM%20field.md), given as it depends on $\underline{A}$, different choices in the gauge give different Hamiltonians while keeping the physical observables the same. It is useful to choose the gauge that yields the simplest Hamiltonian.