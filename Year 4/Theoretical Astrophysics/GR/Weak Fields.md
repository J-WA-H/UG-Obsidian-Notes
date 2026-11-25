From the Lagrangian in the [[Schwarzschild Metric]],
$$L=\frac{1}{2}\left[ \left( 1-\frac{2m}{r} \right)c^2\dot{t}^2-\left( 1-\frac{2m}{r} \right)^{-1}\dot{r}^2-r^2\dot{\phi}^2 \right]\tag{12.1}. $$
As $t,\phi$ don't appear in the Lagrangian, only $\dot{t},\dot{\phi}$, their Euler-Lagrange equations become
$$\frac{d}{ds}\left( \frac{\partial L}{\partial\dot{x}^{\alpha}} \right)=0\implies \frac{\partial L}{\partial \dot{x}^\alpha}=const.\tag{12.2} $$
These coordinates are known as cyclic coordinates. For time and azimuth,
$$\frac{\partial L}{\partial(ct)}=\frac{\partial L}{\partial x^0}=0\implies \frac{\partial L}{\partial \dot{x}^0}=const=\left( 1-\frac{2m}{r} \right)c\dot{t}=g_{00}p^0=p_{0}\tag{12.3}. $$
$$\frac{\partial L}{\partial \phi}=0\implies \frac{\partial L}{\partial \dot{\phi}}=g_{33}p^3=p_{3}\tag{12.4}. $$
As $r\to \infty$, $\left( 1-\frac{2m}{r} \right)p^{0}\to p^{0}=\frac{E_{\infty}}{c}$.
$$\implies\left( 1-\frac{2m}{r} \right)\dot{x}^0=\frac{E_{\infty}}{c}\implies\left( 1-\frac{2m}{r} \right)c^2\dot{t}^2=E\tag{12.5}.$$
$$\frac{\partial L}{\partial \dot{\phi}}=-r^2\dot{\phi}=const\implies r^2\dot{\phi}=L_{z}\tag{12.6}. $$
These cyclic coordinates give conserved quantities, in this case energy and angular momentum. 

In the weak field, we now know $r^2\dot{\phi}=L_{z}$ and $\left( 1-\frac{2m}{r} \right)c^2\dot{t}^2=E$.
$$c^2d\tau^2=\left( 1-\frac{2m}{r} \right)c^2dt^2-\left( 1-\frac{2m}{r} \right)^{-1}dr^2-r^2d\phi^2\tag{12.7} $$
$$\implies c^2=\left( 1-\frac{2m}{r} \right)c^2\left( \frac{dt}{d\tau} \right)^2-\left( 1-\frac{2m}{r} \right)^{-1}\left( \frac{dr}{d\tau} \right)^2-r^2\left( \frac{d\phi}{d\tau} \right)^2=\left( 1-\frac{2m}{r} \right)c^2\dot{t}^2-\left( 1-\frac{2m}{r} \right)^{-1}\dot{r}^2-r^2\dot{\phi}^2\tag{12.8}. $$
$$\implies \frac{c^2}{\dot{\phi}^2}=\left( 1-\frac{2m}{r} \right)c^2\left( \frac{\dot{t}}{\dot{\phi}} \right)^2-\left( 1-\frac{2m}{r} \right)^{-1}\left( \frac{dr}{d\phi} \right)^2-r^2\tag{12.9}. $$
Using $\dot{\phi}=\frac{L_{z}}{r^2}$,
$$\frac{c^2}{\left( \frac{L_{z}}{r^2} \right)^2}=\left( 1-\frac{2m}{r} \right)c^2\left( \frac{\frac{E}{c^2}}{1-\frac{2m}{r}} \right)^2 \frac{1}{\left( \frac{L_{z}}{r^2} \right)^2}-\frac{1}{1-\frac{2m}{r}}\left( \frac{dr}{d\phi} \right)^2-r^2\tag{12.10} $$
$$\frac{c^2r^4}{L_{z}^2}=\frac{c^2r^4}{L_{z}^2} \frac{E^2}{c^4\left( 1-\frac{2m}{r} \right)}-\frac{1}{1-\frac{2m}{r}}\left( \frac{dr}{d\phi} \right)^2-r^2\tag{12.11} $$
$$\frac{\left( 1-\frac{2m}{r} \right)c^2r^4}{L_{z}^2}=\frac{r^4E^2}{L_{z}^2c^2}-\left( \frac{dr}{d\phi} \right)^2-r^2\left( 1-\frac{2m}{r} \right)\tag{12.12} $$
$$\left( \frac{dr}{d\phi} \right)^2=\frac{\left( \frac{E^2}{c^4}-1 \right)c^2r^4}{L_{z}^2}+\frac{2mcr^3}{L_{z}^2}-r^2+2mr\tag{12.13} .$$
This is the equation for an orbit from general relativity.

Compare this to Newtonian results,
$$\tilde{E}=KE+PE,\qquad KE=\frac{1}{2}v^2=\frac{1}{2}(\dot{r}^2+r^2\dot{\phi}^2),\qquad PE=-\frac{Gm}{r}=-\frac{mc^2}{r}\tag{12.14}. $$
This gives
$$\tilde{E}=\frac{1}{2}(\dot{r}^2+r^2\dot{\phi}^2)-\frac{mc^2}{r}\implies \frac{2\tilde{E}}{\dot{\phi}^2}=\left( \frac{\dot{r}}{\dot{\phi}} \right)^2+r^2-\frac{2mc^2}{r\left( \frac{L_{z}}{r^2} \right)^2}\tag{12.15} $$
$$\left( \frac{dr}{d\phi} \right)^2=\frac{2\tilde{E}r^4}{L_{z}^2}-r^2+\frac{2mc^2r^3}{L_{z}^2}\tag{12.16}. $$
The Newtonian result gives closed elliptical orbits. The extra term from GR means the orbit returns after $k\phi=2\pi$ with
$$k=\left( 1-\frac{6GM^2}{L_{z}^2c^2} \right)^{1/2}\approx 2\pi\left( 1+\frac{3G^2M^2}{L_{z}^2c^2} \right)\tag{12.17}. $$
This explains the discrepancy in Mercury's orbit from Newtonian mechanics, with $\Delta \phi=5\times 10^{-7}\text{ rad}$.

Photons are massless so they are not effected by Newtonian gravity, but acceleration is not dependent on mass, so it is effected by general relativity.

To find the photon geodesic,
$$0=\left( 1-\frac{2m}{r} \right)c^2\dot{t}^2-\left( 1-\frac{2m}{r} \right)^{-1}\dot{r}^2-r^2\dot{\phi}^2\tag{12.18}. $$
Set $u=\frac{1}{r}$ so we want $\frac{du}{d\phi}$.
$$\left( \frac{du}{d\phi} \right)^2+u^2=\frac{E^2}{c^2L_{z}^2}+2mu^3\tag{12.19}. $$
For $m\to 0$, we get the weak field limit
$$\left( \frac{du}{d\phi} \right)^2+u^2=\frac{E^2}{c^2L_{z}^2}=u_{0}^2\tag{12.20}. $$
![[Pasted image 20260301105449.png]]
The point of closest approach is $r_{0}=\frac{1}{u_{0}}$ and 
$$\Delta \theta\simeq \frac{4GM}{r_{0}c^2}\tag{12.21}. $$
The maximum deflection is $\sim 1.75''$.
![[Pasted image 20260301105612.png]]
Since we can't see stars this close to the sun in the sky, so can only be observed during a solar eclipse, and compared with results 6-months later. This data agrees with GR instead of Newtonian gravity.