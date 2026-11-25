Consider a particle moving with speed $v$ with respect to some inertial frame $\mathcal{S}$ at two points in spacetime - $x^\mu$ and $x^\mu+\delta x^\mu$.
![[Pasted image 20241019195855.png]]
We can take the [Minkowski scalar product](Lorentz%20Group%20and%20Minkowski%20Scalar%20Product.md) of these two events:
$$\mathcal{S}=(x^\mu-(x^\mu+\delta x^\mu))(x_{\mu}-(x_{\mu}+\delta x_{\mu}))=\delta x^\mu \delta x_{\mu}$$
$$=c^2dt^2-d\underline{x}^2=c^2d\tau^2.$$
The $S'$ frame has been defined to the rest frame of the particle so $d\underline{x}'=0$.
We can rearrange to gain an expression that relates the time experienced in the $S'$ frame to the time experience in the $S$ frame.
$$\left(\frac{d\tau}{dt}\right)^2=1-\frac{1}{c^2}\frac{d\underline{x}}{dt}^2$$
$$\left(\frac{d\tau}{dt}\right)^2=1-\frac{v^2}{c^2}$$
$$\implies d\tau=\sqrt{ 1-\frac{v^2}{c^2} }dt.$$
Integrate through this expression to get:
$$\Delta \tau=\Delta t\sqrt{1-\frac{v^2}{c^2}}=\frac{\Delta t}{\gamma(v(t))}.$$
This implies that a moving clock runs slower than a stationary clock.

This introduces the concept of proper time $\Delta \tau$ - the time experienced by a clock that is stationary with respect to the particle.
 