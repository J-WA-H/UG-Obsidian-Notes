The [[Schwarzschild Metric]] for a particle along a circular path is
$$ds^2=\left( 1-\frac{2m}{r} \right)c^2dt^2-r^2d\phi^2\tag{13.1}. $$
The Lagrangian is then
$$L=\frac{1}{2}\left[ \left( 1-\frac{2m}{r} \right)c^2\dot{t}^2-r^2\dot{\phi}^2 \right]\tag{13.2} $$
Find the Euler-Lagrange equations in $r$, which is simple since there is no $\dot{r}$ dependence,
$$\frac{\partial L}{\partial r}=\frac{1}{2}\left[\left( -\frac{2mr^{-2}}{-1} \right)c^2\dot{t}^2-2r\dot{\phi}^2\right]\tag{13.3}\implies mc^2\dot{t}^2=r^3\dot{\phi}^2 .$$
The period in coordinate time is
$$\frac{d\phi}{dt}=\left( \frac{\dot{\phi}}{\dot{t}} \right)=\left( \frac{mc^2}{r^3} \right)^{1/2}=\left( \frac{Gm}{r^3} \right)^{1/2}\tag{13.4} $$
Integrating this gives with $d\phi=2\pi$,
$$\Delta t=2\pi \left( \frac{r^3}{Gm} \right)^{1/2}\tag{13.5} $$
This is the same period as from Newtonian mechanics. 
![[Pasted image 20260306124930.png]]

For stationary observers,
$$c^2d\tau^2=\left( 1-\frac{2m}{r} \right)c^2dt^2\tag{13.6}. $$
For an stationary observer in frame $S$ at radius $r=r_{0}$,
$$d\tau(S)=\left( 1-\frac{2m}{r_{0}} \right)^{1/2}\Delta t\tag{13.7} $$
At $F$, $r\to \infty$ so
$$d\tau(F)=\left( 1-\frac{2m}{\infty} \right)^{1/2}\Delta t\to\Delta t\tag{13.8} $$
In the frame of an orbiting particle, using $(13.3)$,
$$c^2=\left( 1-\frac{2m}{r} \right)c^2\dot{t}^2-r^2\dot{\phi}^2\tag{13.9}=\left( 1-\frac{2m}{r} \right)c^2\dot{t}^2-r^2 \frac{mc^2\dot{t}^2}{r^3}\implies d\tau=\left( 1-\frac{3m}{r} \right)^{1/2}dt. $$
This shows the period inside of the orbiting spacecraft, in frame $S$, and at $F$ is
$$P(S)=\left( 1-\frac{3m}{r_{0}} \right)^{1/2}\Delta t\tag{13.10}; \qquad P(S)=\left( 1-\frac{2m}{r_{0}} \right)^{1/2}\Delta t ;\qquad P(F)=\Delta t$$
In the spacecraft, the orbiting period goes to zero as $r$ goes to $3m$, and imaginary as $r<3m$.

For general particles, use the full Schwarzschild metric and [cyclic coordinates](Weak%20Fields.md). To find the path we want to find $\dot{r}^2$.
$$c^2=\frac{{\left( 1-\frac{2m}{r} \right)c^2 \frac{E^2}{c^4}}}{\left( 1-\frac{2m}{r} \right)^2}-\frac{\dot{r}^2}{\left( 1-\frac{2m}{r} \right)}-\frac{r^2L_{z}^2}{r^4}\implies c\left( 1-\frac{2m}{r} \right)=\frac{E^2}{c^2}-\dot{r}^2-\frac{L_{z}^2\left( 1-\frac{2m}{r} \right)}{r^2}\tag{13.11}. $$
This gives
$$\dot{r}^2=\frac{E^2}{c^2}-c^2\left( 1-\frac{2m}{r} \right)\left( 1+\frac{L_{z}^2}{c^2r^2} \right)=\frac{E^2}{c^2}-V^2(\vec{r})\tag{13.12}$$
where
$$V^2(r)=c^2\left( 1+\frac{L_{z}^2}{c^2r^2} \right)\left( 1-\frac{2m}{r} \right)\tag{13.13}=c^2\left[ 1-\frac{2GM}{r}+\frac{L_{z}^2}{c^2r^2}-\frac{2GML_{z}^2}{c^2r^3} \right]=c^2-\frac{2c^2GM}{r}+\frac{L_{z}^2}{r^2}-\frac{2GML_{z}^2}{r^3}. $$
In Newtonian gravity, the total energy is
$$\tilde{E}=\frac{1}{2}\left[ \dot{r}^2+r^2\dot{\phi}^2 \right]-\frac{GM}{r}\implies 2\tilde{E}=\dot{r}^2+\frac{r^2L_{z}^2}{r^4}-\frac{2GM}{r}\implies \dot{r}^2=2\tilde{E}-\left[\frac{L_{z}^2}{r^2}-\frac{2GM}{r}\right]\tag{13.14}. $$
The $L_{z}^2$ term represents the centrifugal force, or the angular momentum barrier.

In general relativity we get an extra negative term with a $\frac{1}{r^3}$ dependence, so we want to know where the important tuning points are.
$$\frac{dV^2}{dr}=0=\frac{2m}{r^2}-\frac{2L_{z}^2}{c^2r^3}+\frac{6mL_{z}}{c^2r^4}\implies r^2-\frac{L_{z}^2r}{mc^2}+\frac{3L_{z}^2}{c^2}=0\tag{13.15} .$$
This is a quadratic, which gives
$$r=\frac{L_{z}}{2mc^2}\pm \frac{1}{2}\sqrt{ \frac{L_{z}^2}{m^2c^4}-\frac{12L_{z}^2}{c^2} }=\frac{L_{z}^2}{2mc^2}\pm \frac{L_{z}^2}{2mc^2}\sqrt{ 1-\frac{12m^2c^2}{L_{z}^2}}\tag{13.16}. $$
The stable orbit is the minimum at $r_{+}=\frac{L_{z}^2}{2mc^2}+ \frac{L_{z}^2}{2mc^2}\sqrt{ 1-\frac{12m^2c^2}{L_{z}^2}}$, with the other solution being the unstable orbit. These two merge generating a point of inflection when $1-\frac{12m^2c^2}{L_{z}^2}=0\implies L_{z}=\sqrt{ 12 }mc$.

In Newtonian gravity,
$$V(r)=2\left( -\frac{GM}{r}+\frac{L_{z}^2}{2r^2} \right)\tag{13.17} $$
![[Pasted image 20260308164107.png]]
In general relativity, the gravitational potential energy and the angular momentum barrier terms are the same, but we have a constant shift $c^2$ which we can ignore, and an extra mixed term that adds to gravity.![[Pasted image 20260308164253.png]]
This breaks down the angular momentum barrier. Solutions to the stationary points gives
$$r=\frac{L_{z}^2}{2mc^2}\pm \frac{L_{z}^2}{2mc^2}\sqrt{ 1-\frac{12mc^2}{L_{z}^2} }\tag{13.18} $$
The solutions $r_{+},r_{-}$ are the same when $L_{z}^2=12m^2c^2$. This gives
$$r=\frac{L_{z}^2}{2mc^2}=\frac{12m^2c^2}{2mc^2}=6m\tag{13.19}. $$
This is a point of inflection so no $L$ barrier to stop you falling into the black hole.

However, $r=6m$ is not the event horizon. For a stationary observer,
$$d\tau=\left( 1-\frac{2m}{r} \right)^{1/2}dt,\qquad ds=\left( 1-\frac{2m}{r} \right)^{1/2}cdt\tag{13.20}. $$
The event horizon is when $ds$ turns imaginary so $r=2m$. $r=6m$ is the last / inner most stable circular orbit. The speed on this orbit is
$$v=r\dot{\phi}=r \frac{L_{z}}{r^2}=\frac{L_{z}}{r}\tag{13.21}. $$
Using $L_{z}=\sqrt{ 12}mc$ on the last stable orbit of $r=6m$,
$$v=\frac{\sqrt{ 12 }mc}{6m}=\frac{c}{\sqrt{ 3 }}=0.58c\tag{13.22}. $$
