It is valid to exclude pressure when calculating density perturbations for a normal fluid with zero pressure, like a low temperature gas, and for collisionless fluids with negligible thermal velocity, like CDM.

Recall the [master equation](Linear%20Perturbation%20Equations.md) for $\delta$,
$$\frac{\partial^2\delta}{\partial t^2}+2 \frac{\dot{a}}{a} \frac{\partial\delta}{\partial t}=\frac{\nabla^2_{\vec{x}}\delta p}{a^2\bar{\rho}}+4\pi G\bar{\rho}\delta.\tag{10.6} $$
For zero pressure, $\delta p=0$ so
$$\frac{\partial^2\delta}{\partial t}+2 \frac{\dot{a}}{a} \frac{\partial\delta}{\partial t}=4\pi G\bar{\rho}(t)\delta \tag{11.1} .$$
As everything only depends on time, this can be solved by $\delta(\vec{x},t)=A(\vec{x})D(t)$ where $A(\vec{x})$ is arbitrary. This gives a second order ODE in the linear growth factor $D(t)$,
$$\frac{d^2D}{dt^2}+2H(t) \frac{dD}{dt}-4\pi G\bar{\rho}(t)D(t)=0.\tag{11.2} $$
There are 2 independent solutions, $D_{+}(t),D_{-}(t)$ - one growth and one decay solution. This gives a general solution
$$\delta(\vec{x},t)=A(\vec{x})D_{+}(t)+B(\vec{x})D_{-}(t)\tag{11.3} $$where $A,B$ are determined by initial conditions.
$D_{+}$ is growing in time so this is the growing mode.
$D_{-}$ is decreasing in time so this is the decaying mode.

Gravitational instability is the effect that density perturbations can grow due to their own self gravity.

The decaying mode is generally unimportant as at late times, $\delta \approx A(\vec{x})D_{+}(t)$

The simple form of $\delta$ is only valid in comoving coordinates.
![[Pasted image 20251030164942.png]]
In linear theory, $\delta \rho$ gets stretched with the expansion of the universe, while their amplitude grows or decays.

Consider the non-cosmological case where the background medium is static instead of expanding. This means $a(t)=\text{const.}\implies H=0$, $\bar{\rho}=\text{const.}$ so the master equation becomes
$$\frac{\partial^2\delta}{\partial t^2}-4\pi G\bar{\rho}\delta=0\tag{11.4} $$
This has solutions
$$D_{\pm}(t)\propto e^{ \pm \sqrt{ 4\pi G\bar{\rho} }t }.\tag{11.5} $$
This gives the general solution
$$\delta(\vec{x},t)=A(\vec{x})e^{ t/\tau_{grav} }+B(\vec{x})e^{ -t/\tau_{grav} }\tag{11.6} $$
with
$$\tau_{grav}\equiv \frac{1}{\sqrt{4\pi G\bar{\rho}  }}.\tag{11.7} $$
Now consider the cosmological case in a flat matter-dominated universe where $a\propto t^{2/3},H=\frac{2}{3t}$ and $\bar{\rho}=\frac{1}{6\pi Gt^2}$. Substituting into the master equation gives
$$\frac{d^2D}{dt^2}+\frac{4}{3t} \frac{dD}{dt}-\frac{2}{3t^2}D=0.\tag{11.8} $$
Try a power law solution $D\propto t^{p}$,
$$p(p-1)t^{p-2}+\frac{4}{3}pt^{p-2}-\frac{2}{3}t^{p-2}=0\tag{11.9} $$$$\implies p=\frac{2}{3},\;p=-1\tag{11.10} .$$
This gives the general solution
$$\delta(\vec{x},t)=A(\vec{x})t^{2/3}+B(\vec{x})t^{-1}.\tag{11.11} $$
For large $t$, the growing solution generally dominates so $\delta \approx A(\vec{x})t^{2/3}\propto t^{2/3}\propto a$.

For a flat, vacuum dominated universe, $\rho_{v}\approx\text{const.}$ which is not perturbed $\implies\delta \rho_{v}=0$ and $\delta \rho=\delta \rho_{m}=\bar{\rho}_{m}\delta_{m}$.
Recall vacuum energy only effects perturbation growth through its effect on the overall expansion $a(t)$ and $H(t)$ so the master equation becomes one for $\delta_{m}$,
$$\frac{\partial^2\delta_{m}}{\partial t^2}+2H(t) \frac{\partial\delta_{m}}{\partial t}=4\pi G\bar{\rho}_{m}(t)\delta_{m}.\tag{11.12} $$
Using
$$\bar{\rho}_{m}(t)=\Omega_{m}(t)\rho_{crit}(t)=\Omega_{m}(t) \frac{3H^2(t)}{8\pi G},\tag{11.13} $$
$$\frac{\partial^2\delta_{m}}{\partial t^2}+2H(t) \frac{\partial\delta_{m}}{\partial t}-\frac{3}{2}\Omega_{m}(t)H^2(t)\delta_{m}=0.\tag{11.14} $$
Here $H(a)\approx\text{const.}$ $a\propto e^{ Ht }$ and $\Omega_{m}\ll 1$ so the third term becomes negligible,
$$\frac{\partial^2\delta_{m}}{\partial t^2}+2H \frac{\partial\delta_{m}}{\partial t}=0.\tag{11.15} $$
Separating out into the linear growth function,
$$\frac{d^2D}{dt^2}+2H \frac{dD}{dt}=0\tag{11.16} $$which has solutions
$$D_{+}(t)=\text{const.},\;D_{-}(t)=e^{ -2Ht }.\tag{11.17} $$
$$\therefore \delta_{m}(\vec{x},t)=A(\vec{x})+B(\vec{x})e^{ -2Ht }.\tag{11.18} $$
Here the growing mode is no longer growing but instead constant or 'frozen in', because self-gravity of matter overwhelmed by the expansion of the universe driven by vacuum energy.
![[Pasted image 20251030180149.png]]
We get a power law solution for an expanding universe but exponential in a static universe. The gravitational growth time, $(11.7)$, is similar to the expansion timescale of the universe - $\bar{\rho}(t)$ decreases on similar timescales as that on which the perturbation is trying to grow.

The Hubble drag $2H \frac{\partial\delta}{\partial t}$ retards growth through damping of peculiar velocities (while not existent in a static medium).

Consider a spherical region embedded within this universe, uniformly overdense by $\delta p_{m}>0$:
![[Pasted image 20251030181759.png]]
the acceleration in a flat, matter dominated universe is
$$\frac{\ddot{a}}{a}=-\frac{4\pi G}{3}\bar{\rho}_{m}\tag{11.19} .$$
$\bar{\rho}_{m}>0\implies \ddot{a}<0$, i.e. the expansion of the universe decelerates due to the self gravity of the matter in it.

$a_1(t)$ evolves following the acceleration equation with $\rho_{1}=\bar{\rho}_{m}+\delta \rho_{m}$,
$$\frac{\ddot{a}_{1}}{a_{1}}=-\frac{4\pi G}{3}(\bar{\rho}_{m}+\delta \rho_{m}).\tag{11.20} $$
The region with $\delta \rho_{m}>0$ decelerates more rapidly than a background universe
![[Pasted image 20251030182931.png]]
As $\bar{\rho}_{m}\propto a^{-3}$ and $a_{1}(t)<a(t)\implies$ density $\rho_{1}$ falls less rapidly then $\bar{\rho}_{m}\implies \frac{\delta \rho_{m}}{\bar{\rho}_{m}}$ grows with time due to the effect of its own self-gravity on the expansion.

