#### Vis viva equation
##### Derivation
Start with $\underline{h}\times \dot{\underline{r}}=-\mu(\hat{\underline{r}}+\underline{e})$
Cross with $\underline{h}$ to give
$$\underline{h}\times(\underline{h}\times \dot{\underline{r}})=-\mu \underline{h}\times(\hat{\underline{r}}+\underline{e})$$
$$-h^2\dot{\underline{r}}=-\mu \underline{h}\times(\hat{\underline{r}}+\underline{e})$$
$$\dot{\underline{r}}=\left( \frac{\mu}{h} \right)\hat{\underline{h}}\times(\hat{\underline{r}}+\underline{e})$$
Take dot product of both sides, noting that $\underline{h}$ is out of the plane of motion.
$$|\dot{\underline{r}}|^2=\frac{\mu^2}{h^2}(1+e^2+2e\cos \phi)$$
where $\phi$ is the angle between $\hat{\underline{r}}$ and $\underline{e}$.
Eliminating $e\cos \phi$ from equation ([2](2%20body%20problem%20and%20Kepler's%20laws.md)) gives 
$$|\dot{\underline{r}}|^2=\mu\left( \frac{2}{r}-\frac{{1-e^2}}{p} \right)$$
where $p=\frac{h^2}{\mu}$.
This is the Vis viva equation. and gives the speed of the two objects relative to each other.

Using $p=a(1-e^2)$ gives
$$v^2=\mu\left( \frac{2}{r}-\frac{1}{a} \right)$$
The first time is twice the kinetic energy per unit mass
the second term is twice the potential energy per unit mass
This gives that the final term is twice the total energy per unit mass
$E<0$ implies bound orbit

Parabolic orbit, $e=1$ so $v^2=\mu\left( \frac{2}{r} \right)$
As $r\to \infty$ as $v\to 0$, the escape velocity from $r_{min}$ is $v_{esc}=\sqrt{ \frac{2\mu}{r_{min}} }$.
Hyperbolic orbit, e>1:
As $r\to \infty$, $v\to \sqrt{-\frac{\mu}{a} }$, where $a<0$ from $a=\frac{p}{1-e^2}$.
#### Direction of Velocity
![[Pasted image 20241015130937.png]]
Can find $\theta$ from the radial and tangential components of the velocity via
$$\sin\theta=\frac{r\dot{\phi}}{v}=\frac{h/r}{\sqrt{ \mu\left( \frac{2}{r}-\frac{1}{a} \right) }}.$$
Substituting $h=\sqrt{ \mu a(1-e^2) }$ gives
$$\sin \theta=\left( \frac{a^2(1-e^2)}{r(2a-r)} \right)^{1/2}.$$
At a given point in orbit, the magnitude of the velocity sets $E$, $a$, and $T$. The direction of the velocity sets $e$ and the orientation of the orbit.

Orbits can either be defined by the energy and angular momentum or by the semi-major axis and the eccentricity.