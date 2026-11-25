The wave equation has the form
$$\frac{1}{c^2} \frac{ \partial^2 f }{ \partial t^2 } -\nabla^2f=0.$$
In cartesian coordinates:
$$\nabla^2f=\frac{\partial^2 f}{\partial x^2}+\frac{\partial^2f}{\partial y^2}+\frac{\partial^2f}{\partial z^2}.$$
In spherical coordinates:
$$x=r\cos \phi \sin \theta;\;r=\sqrt{ x^2+y^2+z^2 }$$
$$y=r\sin \phi \sin \theta;\;\theta=\arccos\left( \frac{z}{\sqrt{ x^2+y^2+z^2 }} \right)$$
$$z=r\cos \theta;\;\phi=\arctan\left( \frac{y}{x} \right).$$
$\nabla^2$ can be found using the chain rule.
$$\frac{\partial f}{\partial x}=\frac{ \partial f }{ \partial r } \frac{ \partial r }{ \partial x } +\frac{\partial f}{\partial\theta} \frac{\partial \theta}{\partial x} +\frac{\partial f}{\partial \phi} \frac{\partial \phi}{\partial x}$$
$$\frac{\partial^2f}{\partial x^2}=\frac{\partial}{\partial x}\left( \frac{ \partial f }{ \partial x }  \right).$$
This is also done for $y,z$.

This gives the wave equation:
$$\frac{1}{c^2} \frac{ \partial^2 f }{ \partial t^2 } =\frac{1}{r^2} \frac{\partial}{\partial r}\left( r^2\frac{ \partial f }{ \partial r }  \right)+\frac{1}{r^2\sin \theta} \frac{\partial}{\partial\theta}\left( \sin\theta  \frac{\partial f}{\partial\theta} \right)+\frac{1}{r^2\sin^2\theta} \frac{\partial^2f}{\partial \phi^2}.$$
We want to find $f(r,\theta,\phi,t)=R(r)\Theta(\theta)\Phi(\phi)T(t)$.

This can be used to rewrite the wave equation
$$\frac{1}{c^2} \frac{\ddot{T}}{T}=\frac{1}{r^2R} \frac{\partial}{\partial r}(r^2R')+\frac{1}{r^2\sin \theta} \frac{1}{\Theta} \frac{\partial}{\partial\theta}(\sin \theta \Theta')+\frac{1}{r^2\sin^2 \theta} \frac{\Phi''}{\Phi}.$$
Isolate coordinate derivatives on the LHS.
RHS can be equated with a constant

For $t$:
$$\frac{1}{c^2} \frac{\partial^2f}{\partial t^2}=\nabla^2f=-k^2f$$
where $k$ is constant in time.
$$\frac{1}{c^2} \frac{\ddot{T}}{T}=-k^2\implies \ddot{T}=-c^2k^2T\implies T(t)=T_{0}e^{ \pm ikct }.$$
For $\phi$:
$$\frac{\Phi''}{\Phi}=-m^2=-k^2r^2\sin \theta-\frac{r^2\sin \theta}{r^2R} \frac{d}{dr}(r^2R')-\frac{r^2\sin^2\theta}{r^2\sin \theta\Theta} \frac{d}{d\theta}(\sin \theta\Theta').$$
The RHS is independent of $\phi$
$$\Phi''=-m^2\Phi \implies \Phi_{m}(\phi)=\Phi_{0}e^{ \pm im\phi }.$$
For $\theta$:
$$\frac{1}{\sin\theta\Theta} \frac{d}{d\theta}(\sin\theta\Theta')-\frac{m^2}{\sin^2\theta}=-\frac{1}{R} \frac{d}{dr}(r^2R')-k^2r.$$
Equate LHS to $\ell(\ell+1)$, which is the convention.
$$\frac{1}{\sin \theta} \frac{d}{d\theta}(\sin\theta\Theta')+\left[ \ell(\ell+1)-\frac{m^2}{\sin^2\theta} \right]\Theta=0$$
Introduce $c(\theta)=\cos\theta \implies\Theta=\Theta(\cos\theta)$.
$$\therefore \frac{d\Theta}{d\theta}=\frac{d\Theta}{dc} \frac{dc}{d\theta}=\frac{d\Theta}{dc}(-\sin\theta)=\frac{d\Theta}{dc}(-\sqrt{ 1-c^2 })$$
$$\implies \frac{d^2\Theta}{d\theta^2}=\frac{d}{d\theta}\left( \frac{d\Theta}{dc} \frac{dc}{d\theta} \right)=\frac{d^2\Theta}{dc^2}(1-c^2)+\frac{d\Theta}{dc}(-c).$$
$$\therefore (1-c^2)\Theta''(c)-2c\Theta'(c)+\left( \ell(\ell+1)-\frac{m^2}{1-c^2} \right)\Theta(c)=0.$$
This is the associated Legendre equation.
$P^{m}_{\ell}(\cos \theta)$ are the Legendre polynomials of the first kind.
$Q^{m}_{\ell}(\cos \theta)$ are the Legendre polynomials of the second kind.

For $m=0$, $P^{0}_{\ell}(\cos \theta)=P_{\ell}(\cos \theta)$ are the Legendre polynomials, and $Q_{\ell}$ depends on $\log\left( \frac{{1+\cos \theta}}{1-\cos \theta} \right)$, which causes $(1-c^2)f''(c)-2cf'(c)$ vanish.

For $r$:
$$-\frac{1}{R} \frac{d}{dr}(r^2R')-k^2r^2=\ell(\ell+1).$$
Change variables $s=kr$ so $R'(r)=kR'(s)$ and $R''(r)=k^2R''(s)$.
$$\therefore \frac{d}{dr}(r^2R'(r))=2rR'(r)+r^2R''(r)=\frac{s}{k}kR'(s)+\frac{s^2}{k^2}k^2R''(s)=sR'(s)+s^2R''(s)$$
$$\implies s^2R''(s)+2sR'(s)+(s^2-\ell(\ell+1))R(s)=0.$$
The solutions to this are the spherical Bessel functions.
These are oscillating functions with a decreasing amplitude $\frac{1}{r}$.

This decay relates to geometric spreading due to energy conservation. The area of the wavefront is $4\pi r^2$ and the wave intensity is proportional to the square of the amplitude $|A(r)|^2$.

Intensity is power per unit area
$$\frac{P^2}{4\pi r^2}\implies |A(r)|^2\propto \frac{1}{r^2}\implies |A(r)|\propto \frac{1}{r}.$$
This is for 3 spatial dimensions.
In general,
$$|A(r)|\propto \frac{1}{n^{{n-1}/2}}$$
for $n$ spatial dimensions.