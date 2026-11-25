The [expansion](Expanding%20Universe.md) of the universe is measured from galaxy recession, described by the Hubble flow.

A homogeneous, isotropic, expanding universe necessarily means $\underline{v}=\alpha \underline{r}$ where $\alpha=\alpha(t)$ being a function of time only.
Proof:
Consider the recession of two galaxies from an origin, each at a position of $\underline{r}$ and $\underline{r}'$ respectively, receding at velocities of $v(\underline{r}), v(\underline{r}')$.

![[Pasted image 20250116161329.png]]
The velocity of the primed galaxy with respect to the unprimed galaxy is $v(\underline{r})-v(\underline{r}')=v(\underline{r}-\underline{r}')$ from [homogeneity](Overview%20of%20the%20Universe.md). This shows that $v$ is a linear function of $\underline{r}$.
This implies we write $\underline{v}$ as a matrix equation
$$\underline{v}=\underline{\underline{A}}\underline{r}$$
$$v_{i}=A_{ij}r_{j}.$$
Choose a basis to diagonalise $\underline{\underline{A}}$:
$$\underline{v}=PDP^{-1}\underline{r}$$
$$P^{-1}\underline{v}=DP^{-1}\underline{r}.$$
Define $P^{-1}\underline{v}=\underline{V}$ and $\underline{R}=P^{-1}\underline{r}$.
$$\therefore \underline{V}=\begin{bmatrix}
\alpha & 0 & 0 \\
0 & \beta & 0 \\
0 & 0 & \gamma
\end{bmatrix}\underline{R}.$$
Since the universe is homogeneous, all the diagonal elements are the same, $\alpha=\beta=\gamma$.
$$\therefore \underline{V}=\alpha(t)\underline{R}$$
$$\implies \underline{v}=\alpha(t)\underline{r}\;\square$$
To find $\alpha(t)$ in terms of the [[Cosmic Scale Factor]], consider $r(t)=a(t)r_{0}$.
$$v(t)=\dot{r}(t)=\dot{a}(t)r_{0}=\frac{\dot{a}(t)}{a(t)}a(t)r_{0}=\frac{\dot{a}(t)}{a(t)}r(t)=H(t)r(t)$$
where $\alpha(t)=H(t)=\frac{\dot{a}(t)}{a(t)}$.

$H(t)$ is known as Hubble's parameter, which evaluated at the present day gives Hubble's constant.
Today, 
$$v=H_{0}r.$$
