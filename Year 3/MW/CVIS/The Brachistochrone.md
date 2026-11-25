bn  Consider the [functional](Functionals.md) 
$$S[y]=\int dt\mathcal{L}[y,\dot{y},t].$$
The integrand $\mathcal{L}$ is found by examining the problem - and is often of the form of the Lagrangian,
$$\mathcal{L}=T-V$$
where $T$ is the kinetic energy and $V$ is the potential energy.

The Brachistochrone is a problem proposed by Bernoulli in 1696.
It consists of a bead moving frictionlessly between $A$ and $B$. What is the shape of the wire which minimises the transit time,
![[Pasted image 20250226101258.png]]
The considerations that need to be made are gravitational acceleration, conservation of energy - $\frac{1}{2}mv^2-mgy=\text{constant}$, and which path minimises the time.

Let $T$ be the total transit time,
$$T=\int_{0}^{T}dt=\int_{0}^{D} \frac{ds}{v}$$
where $D$ is the distance between $A$ and $B$, and $v$ is the speed.
we know 
$$ds^2=dx^2+dy^2\implies ds=dx\sqrt{ 1+y'^2(x) }$$
and
$$v^2=\dot{x}^2+\dot{y}^2=
\dot{x}(1+y'^2)=2gy$$from conservation of energy.
This gives
$$T=\int_{x_{a}}^{x_{b}}dx \frac{\sqrt{ 1+y'^2 }}{\sqrt{ 2gy }}$$
Take $$L(x,y,y')=\frac{\sqrt{ 1+y'^2 }}{\sqrt{ 2gy }}.$$
As this is a minimisation problem, use the Euler-Lagrange equation,
$$\frac{d}{dx}\left( \frac{ \partial L }{ \partial y' }  \right)-\frac{ \partial L }{ \partial y } =0.$$
$$\frac{ \partial L }{ \partial y } =-\frac{1}{2}\sqrt{ \frac{{1+y'^2}}{2g} } \frac{1}{y^{3/2}};\;\frac{ \partial L }{ \partial y' }=\frac{y'}{\sqrt{ 2gy(1+y'^2) }}. $$
Substituting this into the Euler-Lagrange equation gives
$$\frac{d}{dx}\left( \frac{y'}{\sqrt{ y(1+y'^2) }} \right)=-\frac{1}{2}\sqrt{ \frac{{1+y'^2}}{y^3} }$$
$$\frac{y''}{\sqrt{ y(1+y'^2) }}-\frac{1}{2} \frac{(y')^2}{\sqrt{ y^3(1+y'^2) }}-\frac{(y')^2y''}{\sqrt{ y(1+y'^2)^3 }}=-\frac{1}{2}\sqrt{ \frac{{1+y'^2}}{y^3} }.$$
Multiply by $\sqrt{ y(1+y'^2) }$,
$$-\frac{1}{2} \frac{{1+y'^2}}{y}=y''-\frac{1}{2} \frac{y'^2}{2y}-\frac{y'^2y''}{1+y'^2}.$$
Multiply by $y(1+y'^2)$,
$$1+2yy''+y'=0$$
Multiply by $y'$,
$$y'+2yy'y''+y'^2=0$$
$$\frac{d}{dx}(y+y'^2y)=0$$
$$\implies y+y'^2y=c$$
$$y'=\sqrt{ \frac{c}{y}-1 }.$$
$$dy=\sqrt{ \frac{{c-y}}{y} }dx \implies x=\int \sqrt{ \frac{y}{c-y} }dy$$
Change variables, $y=c\sin^2\theta$, $dy=2c\sin \theta \cos \theta d\theta.$
$$x=\int \sqrt{ \frac{c\sin^2\theta}{c-c\sin^2\theta} }2c\sin \theta \cos \theta d\theta=\int \sqrt{ \frac{\sin^2\theta}{\cos^2\theta} }2c\sin \theta \cos \theta d\theta=2c\int \tan \theta \cos \theta \sin \theta d\theta$$
$$=2c\int \sin^2\theta d\theta=2c\int \frac{1}{2}-\frac{1}{2}\cos{2}\theta d\theta=c\left( \theta-\frac{1}{2}\sin 2\theta \right)+D.$$
This gives a parametric definition of the curve, which is a cycloid.
$$x=c\left[ \theta=\frac{1}{2}\sin 2\theta \right]+D$$
$$y=c\sin^2\theta=\frac{c}{2}[1-\cos 2\theta].$$
