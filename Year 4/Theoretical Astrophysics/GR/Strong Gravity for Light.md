To find how [[Strong Gravity]] effects light, the aim is to find $\dot{r}$. 
$$ds^2=0=\left( 1-\frac{2m}{r} \right)c^2dt^2-\left( 1-\frac{2m}{r} \right)^{-1}dr^2-r^2d\phi^2=\left( 1-\frac{2m}{r} \right)c^2\dot{t}^2-\left(1- \frac{2m}{r} \right)^{-1}\dot{r}^2-r^2\dot{\phi}^2.\tag{14.1} $$
Using the same cyclic coordinates,
$$\left( 1-\frac{2m}{r} \right)\dot{t}=\frac{E}{c^2},\qquad r^2\dot{\phi}=L_{z}\tag{14.2}. $$
$$\frac{\frac{E^2}{c^2}}{\left( 1-\frac{2m}{r} \right)}-\left( 1-\frac{2m}{r} \right)^{-1}\dot{r}^2-\frac{L_{z}^2}{r^2}=0\tag{14.3} $$
$$\left( 1-\frac{2m}{r} \right)^{-1}\dot{r}^2=\frac{E^2}{c^2} \frac{1}{1-\frac{2m}{r}}-\frac{L_{z}^2}{r^2}\tag{14.4} $$
$$\dot{r}^2=\frac{E^2}{c^2}-\frac{L_{z}^2}{r^2}\left( 1-\frac{2m}{r} \right)=L_{z}^2\left[ \frac{E^2}{L_{z}^2c^2}-\underbrace{ \frac{1}{r^2}\left( 1-\frac{2m}{r} \right)  }_{ V^2(r) }\right]\tag{14.5} $$
where
$$V^2(r)=\frac{\left( 1-\frac{2m}{r} \right)}{r^2}=\frac{1}{r^2}-\frac{2m}{r^3}\tag{14.6} $$
![[Pasted image 20260308171625.png]]
The limits of this are
$$\begin{matrix}
V^2 & \to 0 & \text{as} & r\to 2m \\
 & \to -\infty & \text{as} & r\to 0 \\
 & \to 0 & \text{as} & r\to \infty
\end{matrix}\tag{14.7} .$$
The stationary points can be found by
$$\frac{dV^2}{dr}=-\frac{2}{r^3}+\frac{6m}{r^4}=0\implies-2r^4+6mr^3=0\implies-2r+6m=0\implies r=3m\tag{14.8}. $$
This shows there is one circular orbit for light, at $r=3m$, but this is unstable,
$$V^2_{max}(r=3m)=\frac{\left( 1-\frac{2m}{3m} \right)}{9m^2}=\frac{1}{27m^2}\tag{14.8} $$
If $\frac{E^2}{L_{z}^2c^2}> \frac{1}{27m^2}$, then light can be captured by the Black hole. For light bending in the [[Weak Fields]] limit,
$$\left( \frac{du}{d\phi} \right)^2+u^2=u_{0}^2=\frac{E^2}{c^2L_{z}^2}\tag{14.9} $$
where $r_{0}=\frac{1}{u_{0}}$ is the closest approach (impact parameter).

Consider an observer away from a black hole shining a torch at an angle $\phi$,
![[Pasted image 20260312120648.png]]
We have
$$\tan \phi=\frac{dL}{dR}\tag{14.10}. $$
This uses proper distance $dR$ and proper azimuthal distance $dL$,
$$dR=\left( 1-\frac{2m}{r} \right)^{-1/2}dr,\qquad dL=rd\phi \tag{14.11}. $$
this gives
$$\tan \phi=\frac{rd\phi}{\left( 1-\frac{2m}{r} \right)^{-1/2}dr}=r\left( 1-\frac{2m}{r} \right)^{-1/2} \frac{d\phi}{dr}=r\left( 1-\frac{2m}{r} \right)^{1/2} \frac{\dot{\phi}}{\dot{r}}\tag{14.12} $$
Since $\dot{\phi}=\frac{L_{z}}{r}$ and $\dot{r}=L_{z}\left[ \frac{E^2}{L_{z}^2c^2}-V^2(r) \right]^{1/2}$ for light,
$$\tan \phi=\frac{\left( 1-\frac{2m}{r} \right)}{r\left[ \frac{E^2}{L_{z}^2c^2}-V^2(r) \right]^{1/2}}\tag{14.13}. $$
We know that the orbit for light is when $r=3m$ with $V^2(r=3m)=\frac{1}{27m^2}$, this gives the sizer of the barrier. The light paths are
![[Pasted image 20260312121809.png]]
Light is unaffected in the Newtonian case, for $V^2> \frac{1}{27m^2}$, light flies of to $\pm \infty$, for $V^2=\frac{1}{27m^2}$ we get a circular orbit and for $V^2< \frac{1}{27m^2}$ we get light falling into the black hole.

The black hole's observed size is where the last photon can escape. 
$$\tan \phi_{BH}=\frac{\left( 1-\frac{2m}{r} \right)^{1/2}}{r\left( \frac{1}{27m^2}-V^2 \right)^{2/2}}=\frac{\left( 1-\frac{2m}{r} \right)^{1/2}}{r\left[ \frac{1}{27m^2}-r^{-2}\left( 1-\frac{2m}{r} \right)^{1/2} \right]}\tag{14.14}. $$
The limit as $r\to \infty$ is 
$$\tan \phi_{BH}\sim \phi_{BH}\to\frac{\sqrt{ 27 }m}{r}\tag{14.15}. $$
If light goes in a straight line, we expect $\phi_{BH}=\frac{3m}{r}$, so light travels on a curved path.
![[Pasted image 20260312122637.png]]
