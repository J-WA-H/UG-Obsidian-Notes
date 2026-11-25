### Two-body problem
![[Pasted image 20241013105616.png]]
Two bodies undergo a central force with vector $\underline{r}$.
The equation of motion can be given by
$$\begin{eqnarray}
\ddot{\underline{r}}=-\frac{{G(m_{1}+m_{2})}}{r^2}\underline{\hat{r}}.
\end{eqnarray}$$
Defining $\mu=G(m_{1}+m_{2})$ gives $\ddot{\underline{r}}+\frac{\mu}{r^2}\underline{\hat{r}}=0.$

Taking cross product with separation implies $\underline{r}\times \ddot{\underline{r}}=\underline{0}$. Integrating w.r.t time gives $\underline{r}\times \dot{\underline{r}}=\underline{h}$, with $\underline{h}$ being a constant vector normal to the plane of motion.

Due to conservation of momentum, $r^2\dot{\phi}=h=\text{constant}$.
### Kepler's 2nd law
If two bodies revolve about each other under the influence of a central force, then the line joining them sweeps out equal areas in equal times.

Solving the above differential equation gives
$$\begin{eqnarray}
r=\frac{p}{1+e\cos \phi}
\end{eqnarray}$$
where $p=\frac{h^2}{\mu}$.

$e$ is the eccentricity that defines the shape of the orbit.
For $e<1$, the orbit is an ellipse
For $e=1$, the orbit is a parabola
For $e>1$, the orbit is a hyperbola

$p=a(1-e^2)$ so
$$r=\frac{a(1-e^2)}{1+e\cos \phi}.$$
An ellipse is a closed orbit while a hyperbola asymptotes at and angle of $\pm \theta$ from the orbital axis, where $\cos \theta=\frac{1}{e}$.

A parabola is defined as an infinitely long ellipse of a hyperbola with parallel asymptotes.

Kepler's third law is given by
$$T^2=\frac{4\pi^2a^3}{\mu}.$$