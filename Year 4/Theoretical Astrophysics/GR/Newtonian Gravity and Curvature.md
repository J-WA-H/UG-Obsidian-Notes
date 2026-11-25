Consider two [[Geodesic Paths]] coming from the centre of Earth,
![[Pasted image 20260219113442.png]]
At two points along each geodesic, consider the total force in the y-component,$$2F_{y}=\frac{2GM}{R^2} \frac{y}{R}\tag{8.1}. $$The distance apart is $2y$, and the acceleration is $\frac{d^2y}{dt^2}=-\frac{GM}{R^3}y$.
In special relativity,
$$ds^2=c^2d\tau^2=c^2dt^2-dx^2-dy^2-dz^2\tag{8.2}. $$
In Newtonian mechanics, the spatial separation is small since objects move much slower than the speed of light, so $ds^2\approx c^2d\tau^2$.

Using an affine parameter,
$$\frac{d^2y}{ds^2}=\frac{d^2y}{dt^2}\left( \frac{dt}{ds} \right)^2=\frac{1}{c^2} \frac{d^2y}{dt^2}=-\frac{GM}{c^2R^3}y\tag{8.3}. $$
Comparing this with the [[Riemann Curvature Tensor]],
$$\frac{D^2y}{ds^2}=-R^y_{\;cy{d}}y\dot{x}^c\dot{x}^d\approx-R^y_{\;0y 0}yc^2\implies R^y_{\;0y 0}=\frac{GM}{c^4R^3}\tag{8.4}. $$
This gives tidal forces, $\frac{GM}{R^3}$.

Consider geodesics on a sphere,
![[Pasted image 20260219115134.png]]
If we take the tensor around a loop,
$$\lambda^a(loop)-\lambda^a(start)=\Delta\lambda^a(loop)=-\frac{1}{2}(R^a_{\;bcd})_{P}\lambda^bf^{cd}\tag{8.5} $$which shows that the Riemann curvature tensor also describes the space swing on a curved surface. $f^{cd}$ is the area enclosed by the loop.

The curvature tensor also describes covariant derivates. If we take two covariant derivatives,
$$\lambda^{a}_{\;;bc}-\lambda^{a}_{\;;cb}=-R^{a}_{\;dbc}\lambda^{d}\tag{8.6} $$which shows these derivatives can be determined just from the curvature tensor, but as a consequence we get tidal forces from gravity.
