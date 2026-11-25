There are some special radii around a black hole from [[Strong Gravity]],
- $r=6m$ - the last stable orbit for particles
- $r=3m$ - orbit for light
- $r=2m$ - no such thing as a stationary observer. There is also infinite gravitational redshift.

Gravitational redshift is given by
$$\frac{\nu_{R}}{\nu_{E}}=\left( \frac{{1-\frac{2m}{r_{E}}}}{1-\frac{2m}{r_{R}}} \right)^{1/2}\tag{15.1} $$
For $r_{R}\to \infty$,
$$\nu_{R}\to \nu_{E}\left( 1-\frac{2m}{r_{E}} \right)^{1/2}.\tag{15.2} $$
This goes imaginary for $r_{E}<2m$ which is not physical. There are no real paths for $r<2m$.

The [[Schwarzschild Metric]] 
$$ds^2=c^2d\tau^2=\left( 1-\frac{2m}{r} \right)c^2dt^2-\left( 1-\frac{2m}{r} \right)^{-1}dr^2-r^3d\phi^2\tag{15.3} $$
shows there is no stationary real paths for $r<2m$. For $r<2m$, time and space swap signs, so swap characteristics.

Moving forwards in time means moving inwards in space.

Consider plunging into a black hole
![[Pasted image 20260312124144.png]]
$$c^2=\left( 1-\frac{2m}{r} \right)c^2\dot{t}^2-\left( 1-\frac{2m}{r} \right)^{-1}\dot{r}^2\tag{15.4} $$
Using conserved quantities, and assuming you were dropped from rest at $r=r_{0}$,
$$c^2=\left( 1-\frac{2m}{r_{0}} \right)c^2\dot{t}^2\implies \dot{t}^2=\frac{1}{\left( 1-\frac{2m}{r_{0}} \right)}\tag{15.5} .$$
As $r_{0}\to \infty$, $\dot{t}^2\to 1$.

This implies
$$\left( 1-\frac{2m}{r_{0}} \right)\dot{t}=\frac{E}{c^2}\to 1\tag{15.6}. $$
This holds everywhere. This then gives
$$c^2=\left( 1-\frac{2m}{r} \right)c^2 \frac{1}{\left( 1-\frac{2m}{r} \right)^2}-\frac{\dot{r}^2}{\left( 1-\frac{2m}{r} \right)}\tag{15.7} $$
$$\implies c^2\left( 1-\frac{2m}{r} \right)=c^2-\dot{r}^2\implies c^2-\frac{2mc^2}{r^2}=c^2-\dot{r}^2\implies \dot{r}=\pm \sqrt{ \frac{2m}{r} }c\tag{15.8}. $$
Since we are falling towards the black hole, take $\dot{r}<0$.
$$\dot{r}=\frac{dr}{d\tau}=-\sqrt{ \frac{2mc^2}{r} }=-\left( \frac{2GM}{r} \right)^{1/2}\tag{15.9} .$$
This is similar to the Newtonian case, but we are dealing in proper time.
$$\frac{dr}{d\tau}=-\sqrt{ 2m }c \frac{1}{r^{1/2}}\tag{15.10}. $$
This gives
$$\int_{r}^{r_{0}}r^{1/2}dr=\sqrt{ 2m }c\int_{0}^{\tau}d\tau \implies \tau=\frac{2}{3c\sqrt{ 2m }}[r_{0}^{3/2}-r^{3/2}]\tag{15.11}. $$
This shows that nothing strange happens in the rest frame as $r\to 2m$.

At infinity, a stationary observer has $d\tau=dt$. Measure the radial velocity as
$$\frac{dr}{dt}=\frac{dr}{d\tau} \frac{d\tau}{dt}=-\sqrt{ \frac{2m}{r} }c\left( 1-\frac{2m}{r} \right)\tag{15.12} .$$
This goes to zero as $r\to 2m$.
![[Pasted image 20260312165604.png]]
A spacecraft falling into a black hole is described by a diagram.
![[Pasted image 20260330101851.png]]
If the spacecraft emitted a light beam to $\infty$, 
$$0=\left( 1-\frac{2m}{r} \right)c^2dt^2-\left( 1-\frac{2m}{r} \right)^{-1}dr^2\implies \frac{dr}{dt}=\pm\left( 1-\frac{2m}{r} \right)c\implies \frac{dr}{1-\frac{2m}{r}}=c\frac{d}{dt} \tag{15.13} $$
This shows that $cdt\to \infty$ as $r\to 2m$.

To describe the Horizon, we need to consider the Schwarzschild metric. From the radial term, there is a singularity at $r=2m$.
![[Pasted image 20260330102834.png]]
The paths are singular at the pole, $\phi=0\to 2\pi$ does not change position. Any $\phi$ maps to the same point. This is a coordinate singularity.

We aim to determine if the metric singularity is a true or coordinate singularity.

From the [Ricci tensor](Einstein%20Equation.md), all components are zero in empty space. Considering the full [[Riemann Curvature Tensor]], the curvature scalar is $\frac{1}{r^{6}}$ for the Schwarzschild metric. There is no real curvature singularity at $r=2m$, on the only singularity is at $r\to0$.

The embedding diagram is
![[Pasted image 20260330104003.png]]
The horizon is where light can no longer escape, matter coming in can fall straight through. At $r=2m$, a path at $45^\circ$ forms a lightcone so can no longer reach infinity.
