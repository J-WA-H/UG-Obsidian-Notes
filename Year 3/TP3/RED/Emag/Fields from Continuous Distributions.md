In the case of static charges with the [[Lorenz Gauge]]:
$$\nabla^2\phi=-\frac{\rho}{\varepsilon_{0}};\;\nabla^2\underline{A}=-\mu_{0}\underline{j}.$$
This gives 4 Poisson equations - one for $\phi$ and 3 for the spatial dimensions of $\underline{A}$, the solutions of which take the form 
$$\phi(\underline{r})=\frac{1}{4\pi\varepsilon_{0}}\int_{V} \frac{\rho(r')}{\lvert \underline{r}-\underline{r}' \rvert }dV'$$
$$\underline{A}(\underline{r})=\frac{\mu_{0}}{4\pi}\int_{V} \frac{\underline{j}(r')}{\lvert \underline{r}-\underline{r}' \rvert }.$$
![[Pasted image 20241102081437.png]]
Consider the distance between the observer and source: $R=\lvert \underline{r}-\underline{r}' \rvert$.

Sometimes it is easier to measure the time information left the source, rather than the time it arrives at the observer. This is known as the retarded time
$$t_{r}=t-\frac{R}{c}.$$
Note retarded time is also dependent of the position of the observer $\underline{r}$ as well as t.
We can use this to generalise the previous solutions for the potentials - known as the retarded potentials:
$$\phi(\underline{r},t)=\frac{1}{4\pi\varepsilon_{0}} \int_{V'} \frac{\rho(\underline{r}',t_{r})}{R}dV'$$
$$\underline{A}(\underline{r},t)=\frac{\mu_{0}}{4\pi} \int_{V'} \frac{\underline{j}(\underline{r}',t_{r})}{R}dV'.$$
Now check the retarded potentials follow the [evolution equation](Lorenz%20Gauge.md), $\square \phi=\frac{\rho}{\varepsilon_{0}}$.
$$\frac{\partial^2\phi}{\partial t^2}-\nabla^2\phi=\frac{\rho}{\varepsilon_{0}}.$$
First compute $\underline{\nabla}\phi$.
$$\underline{\nabla}\phi=\frac{1}{4\pi\varepsilon_{0}}\int_{V'}(\underline{\nabla}\rho) \frac{1}{R}+\rho\underline{\nabla}\left( \frac{1}{R} \right)dV'.$$
By the chain rule:
$$\underline{\nabla}\rho= \frac{\partial\rho}{\partial t_{r}}\underline{\nabla}t_{r}=-\frac{1}{c} \frac{\partial \rho}{\partial t}\underline{\nabla}R.$$
Using results from vector calculus
$$\underline{\nabla}R=\underline{\hat{R}},\;\underline{\nabla}\left( \frac{1}{R} \right)=-\frac{\underline{\hat{R}}}{R^2}.$$
This gives
$$\underline{\nabla}\phi=\frac{1}{4\pi\varepsilon_{0}} \int_{V'}\left[ -\frac{\dot{\rho}}{c} \frac{\underline{\hat{R}}}{R}-\frac{\rho \underline{\hat{R}}}{R^2} \right]dV'.$$
Now calculate $\nabla^2\phi=\underline{\nabla}\cdot \underline{\nabla}\phi$:
$$\nabla^2\phi=\frac{1}{4\pi\varepsilon_{0}}\int_{V'}\left( -\frac{1}{c}\left[ \frac{\underline{\hat{R}}}{R}\cdot(\underline{\nabla}\dot{\rho})+\dot{\rho}\underline{\nabla}\cdot\left( \frac{\underline{\hat{R}}}{R} \right) \right] -\left[ \frac{\underline{\hat{R}}}{R^2}\cdot(\underline{\nabla}\rho)+\rho \underline{\nabla}\cdot\left( \frac{\underline{\hat{R}}}{R^2} \right) \right]\right)dV'.$$
$$\underline{\nabla}\dot{\rho}=-\frac{1}{c}\ddot{\rho}=-\frac{1}{c}\ddot{\rho}\underline{\nabla}R=-\frac{1}{c}\ddot{\rho}\underline{\hat{R}}.$$
Plugging this into $\nabla^2\phi$ using $\underline{\hat{R}}\cdot \underline{\hat{R}}=1$ so we can write
$$-\frac{1}{c} \frac{\underline{\hat{R}}}{R}\cdot(\underline{\nabla}\rho)=\frac{1}{c^2R} \frac{\partial^2\rho}{\partial t^2}.$$
The second and third terms cancel, which can be seen by the equation for $\underline{\nabla}\rho$.
To rewrite the fourth term, we use the result
$$\underline{\nabla}\cdot\left( \frac{\underline{\hat{R}}}{R^2} \right)=4\pi \delta^3(\underline{R}).$$
Explicitly writing the $\underline{r}$, $\underline{r}'$ dependence we get the forth term as
$$-\rho(\underline{r}',t_{r})\underline{\nabla}\cdot\left( \frac{\underline{\hat{R}}}{R^2} \right)=-\rho(\underline{r}',t_{r})4\pi\delta^3(\underline{r}-\underline{r}').$$
This gives
$$\nabla^2\phi=\frac{1}{4\pi\varepsilon_{0}} \int_{V'}\left[ \frac{1}{c^2R} \frac{\ddot{\rho}}{R}-4\pi \rho \delta^3(\underline{r}-\underline{r}') \right]dV'$$
$$=\frac{1}{4\pi\varepsilon_{0}}\left[\frac{1}{c^2}\int_{V'} \frac{\ddot{\rho}}{R}dV'+\int_{V'} 4\pi \rho\delta^3(\underline{r}-\underline{r}')dV' \right]$$
$$=\frac{1}{c^2} \frac{\partial^2\phi}{\partial t^2}-\frac{\rho(\underline{r}',t)}{\varepsilon_{0}}\;\square$$
So $\phi$ satisfies the evolution equation for the Lorentz Gauge.