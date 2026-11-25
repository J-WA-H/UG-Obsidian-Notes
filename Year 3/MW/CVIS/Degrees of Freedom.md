Degrees of freedom, or generalised coordinates, are physically relevant variables, e.g. position, charge, and spin.
In thermodynamics, degrees of freedom tells you about the distribution of energy in a system.

Some dof may not be important for a problem.
Sometimes a change of variable is necessary to uncover the minimal degrees of freedom.

Example: Double pendulum
![[Pasted image 20250305101508.png]]
Consider two pendulums joint together, the total length $l$ and each one has length $l_{1},l_{2}$ respectively. 
$l_{1},l_{2}$ do not change so we have two degrees of freedom - $\theta_{1},\theta_{2}$.
Set up the Lagrangian,
$$T=\frac{1}{2}m_{1}(\dot{x}_{1}^2+\dot{y}_{1}^2)+\frac{1}{2}m_{2}(\dot{x}^2_{2}+\dot{y}_{2}^2)$$
$$x_{1}=l_{1}\sin\theta_{1};\;x_{2}=l_{1}\sin\theta_{1}+l_{2}\sin\theta_{2}$$
$$y_{1}=l_{1}\cos\theta_{1};\;y_{2}=l_{1}\cos\theta_{1}+l_{2}\cos\theta_{2}$$
$$\dot{x}_{1}=l_{1}\dot{\theta}_{1}\cos\theta_{1};\;\dot{x}_{2}=l_{1}\dot{\theta}_{1}\cos\theta_{1}+l_{2}\dot{\theta}_{2}\cos\theta_{2}$$
$$\dot{y}_{1}=-l_{1}\dot{\theta}_{1}\sin\theta_{1};\;\dot{y}_{2}=-l_{1}\dot{\theta}_{1}\sin\theta_{1}-l_{2}\dot{\theta}_{2}\sin\theta_{2}.$$
$$\therefore (\dot{x}_{2}^2+\dot{y}_{2}^2)=(l_{1}\dot{\theta}_{1})^2+(l_{2}\dot{\theta}_{2})^2+2l_{1}l_{2}\dot{\theta}_{1}\dot{\theta}_{2}(\cos\theta_{1}\cos\theta_{2}+\sin\theta_{1}\sin\theta_{2})$$
$$\implies T=\frac{1}{2}(m_{1}+m_{2})l_{1}^2\dot{\theta}^2_{1}+\frac{1}{2}m_{2}\dot{\theta}_{2}^2l_{2}^2+m_{2}l_{1}l_{2}\dot{\theta}_{2}\dot{\theta}_{1}\cos(\theta_{1}-\theta_{2}).$$
$$V=-g(m_{1}y_{1}+m_{2}y_{2})=-g(m_{1}l_{1}+m_{2}l_{2})\cos\theta_{1}-m_{2}gl_{2}\cos\theta_{2}.$$
Example: Disk running down a slope
![[Pasted image 20250305102545.png]]
$x$ is the distance rolled and $\phi$ is the rotation of the disk of radius $a$.
$$T=\frac{1}{2}m\dot{x}^2+\frac{1}{2}I\dot{\phi}^2.$$
For a disk, $I=\frac{1}{2}ma^2$.
$$\therefore \frac{1}{2}m\dot{x}^2+\frac{1}{4}ma^2\dot{\phi}^2.$$
$$V=-mgx\sin \theta.$$
$$\therefore \mathcal{L}=T-V=\frac{1}{2}m\dot{x}^2+\frac{1}{4}ma^2\dot{\phi}^2+mgx\sin \theta$$
Using $x=a\phi$,
$$\mathcal{L}=\frac{3}{2}ma^2\dot{\phi}^2+mga\phi \sin \theta$$
This is an equation in $\phi$ only.
In $x$ only this becomes,
$$\mathcal{L}=\frac{3}{4}m\dot{x}^2+mgx\sin \theta.$$
Using the [Euler-Lagrange equation](Functionals.md),
$$\frac{d}{dt}\left( \frac{3}{2}m\dot{x} \right)=\frac{3}{2}m\ddot{x}=mg\sin \theta$$
$$\ddot{x}=\frac{2}{3}g\sin \theta.$$
Solving this gives
$$x(t)=\frac{1}{3}g\sin \theta t^2+ct+d.$$
Extended systems have internal degrees of freedom but we can simplify by integrating our details that are irrelevant.

Example: Pendulum rod
Assume the rod density is uniform, $\rho=\frac{M}{L}$.
![[Pasted image 20250305103545.png]]
To describe the motion we only need $\theta$.
Consider a small segment $\delta r$ which has mass $\delta m=\rho\delta r$
$$\delta T=\frac{1}{2}\delta m(\dot{x}^2+\dot{y}^2)=\frac{1}{2}\delta m(r^2\dot{\theta}^2)=\frac{1}{2}\rho\delta rr^2\dot{\theta}.$$
$$\delta V=-\delta mgr\cos \theta=-\rho gr\cos \theta\delta r$$
Integrate over length to find the length of the pendulum,
$$T=\int_{0}^{L}dr \frac{1}{2}\rho r^2\dot{\theta}^2=\left[ \frac{1}{6}\rho r^2\dot{\theta}^2 \right]_{0}^{L}=\frac{1}{6}\rho L^3\dot{\theta}^2=\frac{1}{6}mL^2\dot{\theta}^2.$$
$$V=\int_{0}^{L}dr\rho gr\cos \theta=\left[ -\rho g \frac{r^2}{2}\theta \right]_{0}^{L}=\frac{1}{2}\rho gL^2\cos \theta=-\frac{1}{2}mgL\cos \theta.$$

$$\therefore \mathcal{L}=\frac{1}{6}mL^2\dot{\theta}^2+\frac{1}{2}mgL\cos \theta$$
EL:
$$\frac{1}{2}\cancel{m}L^{\cancel{2}}\ddot{\theta}=\frac{1}{2}\cancel{m}g\cancel{L}\sin \theta \implies \ddot{\theta}=\frac{3}{2} \frac{g}{L}\sin \theta.$$
