The restricted 3-body problem consists of two massive bodies in circular orbits about a common centre of mass with a small body of negligible mass in a combined gravitational field.

To set up this problem, we will choose units such that the total mass of the two massive bodies is 1 so the more massive one has mass $1-m$ and the less massive one has mass $m$, $G=1$, and the separation of these bodies are 1. All motion will be constrained to a single plane.
![[Pasted image 20241025134615.png]]
$(x_{0},y_{0})$ are the coordinates in the inertial frame and $(x,y)$ are the coordinates in the frame rotating with the two massive bodies. 
The coordinate transform between these two frames is given by
$$x_{0}=x\cos(\omega t)-y\sin(\omega t)$$
$$y_{0}=x\sin(\omega t)-y\cos(\omega t).$$
From the choice of units, $\omega=1$.
The fixed coordinates of the massive particles are at $(x_1,0)$ and $(x_2,0)$ respectively, while the small mass is at position $(x(t),y(t))$.
This distance between the small mass and each massive mass is given by:
$$r_1=[(x-x_{1})^2+y^2]^{1/2}$$
$$r_{2}=[(x-x_{2})^2+y^2]^{1/2}.$$
The kinetic energy of the small mass in this reference frame is given by
$$T=\frac{m'}{2}(\dot{x}_{0}^2+\dot{y}_{o}^2)=\frac{m'}{2}((\dot{x}-y)^2+(\dot{y}+x)^2)$$and the potential is given by
$$V=-m'\left( \frac{{1-m}}{r_{1}}+\frac{m}{r_{2}} \right).$$
This yields the Lagrangian
$$\mathcal{L}(x,y,\dot{x},\dot{y})=\frac{m'}{2}[(\dot{x}-y)^2+(\dot{y}+x)^2]$$
which plugging into the Euler-Lagrange equation yields the system of differential equations
$$\ddot{x}-2\dot{y}=x-{\frac{(1-m)(x-x_{1})}{r_{1}^3}}-\frac{m(x-x_{2})}{r_{2}^3}$$
$$\ddot{y}+2\dot{x}=y-\frac{(1-m)y}{r_{1}^3}-\frac{m(x-x_{2})}{r_{2}^3}.$$
The $2\dot{y}$, $2\dot{x}$ terms show the Coriolis force, the isolated $x$, $y$ terms show the centrifugal force and the rest of the terms represent the gravitational force. These ODEs cannot always be solved analytically but we can still gain intuition from them.
Define an effective potential
$$U=\frac{1}{2}(x^2+y^2)+\frac{{1-m}}{r_{1}}+\frac{m}{r_{2}}.$$
This simplifies are equations to
$$\ddot{x}-2\dot{y}=\frac{\partial U}{\partial x}$$
$$\ddot{y}+2\dot{x}=\frac{\partial U}{\partial y}.$$
Cancelling the $\dot{x}$, $\dot{y}$ terms gives
$$2\dot{x}\ddot{x}+2\dot{y}\ddot{y}=2\dot{x} \frac{\partial U}{\partial x}+2\dot{y} \frac{\partial U}{\partial y}$$
$$\frac{d}{dt} (\dot{x}^2+\dot{y}^2)=2 \frac{dx}{dt} \frac{\partial U}{\partial x}+2 \frac{dy}{dt} \frac{\partial U}{\partial y}=\frac{d}{dt} (2U).$$
Integrating this equation w.r.t time gives
$$v^2=2U-C.$$
This is Jacobi's integral and $C$ is Jacobi's constant.

Since $v^2\geq 0$, $m'$ stays in the region where $2U \geq C$. These regions are bound by the zero velocity surfaces satisfying 
$$(x^2+y^2)+\frac{2(1-m)}{r_{1}}+\frac{2m}{r_{2}}=C.$$
Lagrange points are positions where $U$ is stationary
$$\frac{\partial U}{\partial x}=\frac{\partial U}{\partial y}=0.$$
$$\implies x-\frac{(1-m)(x-x_{1})}{r_{1}^3}-\frac{m(x-x_{2})}{r_{2}^3}=0$$
$$y-\frac{(1-m)y}{r_{1}^3}-\frac{my}{r_{2}^3}=0.$$
These equations shows at Lagrange points, $\ddot{x}-2\dot{y}=\ddot{y}+2\dot{x}=0$.
![[Pasted image 20241025152001.png]]
The contours show constant $U$ and Lagrange points are shown. 
Solving the above equations give the positions of L1, L2 and L3,
$$d_{1}=\left( \frac{m}{3} \right)^{1/3}-\frac{1}{3}\left( \frac{m}{2} \right)^{2/3}-\frac{1}{9}\left( \frac{m}{3} \right)$$
$$d_{2}=\left( \frac{m}{3} \right)^{1/3}+\frac{1}{3}\left( \frac{m}{3} \right)^{2/3}-\frac{1}{9}\left( \frac{m}{3} \right)$$
$$d_{3}=2-\frac{7}{12}m-\frac{1127}{20736}m^3.$$
