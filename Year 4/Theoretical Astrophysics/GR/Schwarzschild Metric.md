In 4D spacetime, the [[Einstein Equation]] gives 16 equations, which, from symmetries, reduces to 10.

Pick a simple situation to compare with Newtonian gravity, e.g. a static spherically symmetric mass.
$$\implies ds^2=A(r)c^2dt^2-B(r)dr^2-r^2d\theta^2-r^2\sin^2\theta d\phi^2\tag{11.1} $$
We can form a Lagrangian
$$\mathcal{L}=\frac{1}{2}g_{\mu \nu}\dot{x}^{\mu}\dot{x}^{\nu}=\frac{1}{2}[Ac^2\dot{t}^2-B\dot{r}^2-r^2\dot{\theta}^2-r^2\sin^2\theta \dot{\phi}^2]\tag{11.2}. $$
Then use the Euler-Lagrange equations, which gives the [[Geodesic Paths]] that constrain $A, \frac{dA}{dr}, B, \frac{dB}{dr}$.
$$R^{\mu \nu}=\kappa\left( T^{\mu \nu}-\frac{1}{2}g^{\mu \nu}T \right)=0\tag{11.3} $$
in empty space. This gives
$$A=1+\frac{k}{r},\qquad B=\frac{1}{A}\tag{11.4}$$
with the weak field connections giving
$$k=-\frac{2GM}{c^2}=-2m.\tag{11.5} $$
This gives the metric
$$ds^2=\left( 1-\frac{2m}{r} \right)c^2dt^2-\left( 1-\frac{2m}{r} \right)^{-1}dr^2-r^2d\theta^2-r^2\sin^2\theta d\phi^2\tag{11.6}. $$
Going back to the Einstein field equations gives
$$\kappa=-\frac{8\pi G}{c^4}\tag{11.7} $$
which gives
$$R^{\mu \nu}-\frac{1}{2}g^{\mu \nu}R=-\frac{8\pi G}{c^4}T^{\mu \nu}\tag{11.8} $$
As $m\to{0}$, the Schwarzschild metric gives the Minkowski metric. In the rest frame, we have measured proper time but $dr=d\theta=d\phi=0$,
$$ds^2=c^2dt^2\tag{11.9} $$
For a non-zero mass,
$$ds^2=\left( 1-\frac{2m}{r} \right)c^2dt^2\tag{11.10}. $$This shows that proper time is warped, as it is not equal to coordinate time.

In special relativity, proper distance supresses the negative sign in the metric. $dt=0$ as proper distance is measuring the length between two points at the same time.
$$dR^2=dr^2+r^2d\theta^2+r^2\sin^2\theta d\phi^2\tag{11.11} $$
for $m\to 0$. For $d\theta=d\phi=0$, $dR^2=dr^2$. The radial proper distance is the radial coordinate. For $m\neq 0$,
$$dR^2=\left( 1-\frac{2m}{r} \right)^{-1}dr^2\tag{11.12} $$
which shows that proper distance is also warped.

This warping is shown by an embedding diagram
![[Pasted image 20260226120041.png]]
This shows the warping of space. For stationary observers, $dr=d\theta=d\phi=0$,
$$\therefore ds^2=\left( 1-\frac{2m}{r} \right)c^2dt^2\tag{11.13}. $$
This gives
$$d\tau=\sqrt{ 1-\frac{2m}{r} }dt\tag{11.14} ,$$
this is positive for $r>2m$, and goes imaginary for $r<2m$, which implies there is no real path for stationary observers for $r<2m$, you have to be moving in space to smaller $r$. This describes black holes, with radius
$$r=2m=\frac{2GM}{c^2}\tag{11.15}. $$
General paths change in radius and azimuth ($r,\phi$) but not in $\theta$. Set $\theta=\frac{\pi}{2}$.
$$\implies ds^2=\left( 1-\frac{2m}{r} \right)c^2dt^2-\left( 1-\frac{2m}{r} \right)^{-1}dr^2-r^2d\phi^2\tag{11.16}.$$
This is the form of the metric for particle. For light, $ds^2=0$.
![[Pasted image 20260226120628.png]]
At the circle,
$$ds^2=\left( 1-\frac{2m}{r_{0}} \right)c^2dt^2-r_{0}^2d\phi^2\tag{11.17}. $$
For radial particle paths,
$$ds^2=\left( 1-\frac{2m}{r} \right)c^2dt^2-\left( 1-\frac{2m}{r} \right)^{-1}dr^2\tag{11.18} $$
while radial light paths gives
$$ds^2=0=\left( 1-\frac{2m}{r} \right)c^2dt^2-\left( 1-\frac{2m}{r} \right)^{-1}dr^2\tag{11.19}. $$
This can be used to consider gravitational redshift. 
![[Pasted image 20260226121236.png]]
For emitted light,
$$\left( 1-\frac{2m}{r_{E}} \right)c^2dt_{E}^2=\left( 1-\frac{2m}{r_{E}} \right)^{-1}dr_{E}^2\implies cdt_{E}=\left( 1-\frac{2m}{r_{E}} \right)^{-1}dr_{E}\tag{11.20} $$
For the received light
$$cdt_{R}=\left( 1-\frac{2m}{r_{R}} \right)^{-1}dr_{R}\tag{11.21}. $$
We can get the coordinate speed of light,
$$\frac{dr}{dt}=\pm c\left( 1-\frac{2m}{r} \right)\tag{11.22}. $$
$$\int_{r_{E}}^{r_{R}} \frac{dr}{1-\frac{2m}{r}}=\int_{t_{E}}^{t_{R}}cdt\tag{11.23}. $$
This gives
$$c(t_{R}-t_{E})=\int_{R_{E}}^{R_{R}} \frac{dr}{1-\frac{2m}{r}}\tag{11.24}. $$
For a second photon,
$$c(t_{R_{2}}-t_{E_{2}})=\int_{R_{E_{2}}}^{R_{R_{2}}} \frac{dr}{1-\frac{2m}{r}}\tag{11.25}. $$
Since they are emitted and received at the same radii, $t_{R_{1}}-t_{E_{1}}=t_{R_{2}}-t_{E_{2}}$ which gives $\underbrace{ t_{R_{2}}-t_{R_{1}} }_{ r_{R} }=\underbrace{ t_{E_{2}}-t_{E_{1}} }_{ r_{E} }$.
For an observer fixed at $r_{R}$,
$$ds^2=\left( 1-\frac{2m}{r_{R}} \right)c^2dt^2\implies d\tau=\left( 1-\frac{2m}{r_{R}} \right)^{1/2}dt\tag{11.26}. $$
$$\implies \frac{\Delta \tau_{E}}{\Delta\tau_{R}}=\left( \frac{{1-\frac{2m}{r_{E}}}}{1-\frac{2m}{r_{R}}} \right)^{1/2}=\frac{\nu_{R}}{\nu_{E}}\tag{11.27}. $$
For $r_{R}\to \infty$, $\nu_{R}=\nu_{E}\left( 1-\frac{2m}{r_{E}} \right)^{1/2}<\nu_{E}$.
