Constants are defined as expressions where the derivative with respect to internal variables is zero.
The full derivative is defined by
$$\frac{d\mathcal{L}}{dx}=\frac{\partial \mathcal{L}}{\partial x}+\frac{ \partial \mathcal{L} }{ \partial y }y'+\frac{ \partial \mathcal{L} }{ \partial y' }y''.  $$
If $\frac{ \partial \mathcal{L} }{ \partial x }=0$ and $\frac{ \partial \mathcal{L} }{ \partial y }=\frac{d}{dx}\left( \frac{\partial \mathcal{L}}{\partial y'} \right)$,
$$\implies \frac{d\mathcal{L}}{dx}=\frac{d}{dx}\left( \frac{\partial \mathcal{L}}{\partial y'} \right)y'+\frac{\partial \mathcal{L}}{\partial y'}y''=\frac{d}{dx}\left( y' \frac{\partial \mathcal{L}}{\partial y'} \right)$$
$$\implies \frac{\partial \mathcal{L}}{\partial x}-\frac{d}{dx}\left( y'\frac{\partial \mathcal{L}}{\partial y'} \right)=0=\frac{d}{dx}\left( \mathcal{L}-y' \frac{\partial \mathcal{L}}{\partial y'} \right)$$
This shows that $\mathcal{L}-y' \frac{\partial \mathcal{L}}{\partial y'}$ is a conserved quantity.

If $\mathcal{L}$ is independent of $y$ then $\frac{\partial \mathcal{L}}{\partial y'}$ is constant.

This is Noether's theorem.

An application of this is [planetary motion](2%20body%20problem%20and%20Kepler's%20laws.md). 
To evaluate the motion of a planet's orbit, first form its Lagrangian.
$$T=\frac{1}{2}m(\dot{r}^2+r^2\dot{\phi}^2).$$
$$V=-\frac{GMm}{r}\implies \mathcal{L}=T-V=m\left( \frac{1}{2}\dot{r}^2+\frac{1}{2}r^2\dot{\phi}^2+\frac{GM}{r} \right).$$
$\mathcal{L}$ is independent of $t$ and $\phi$ which leads to 3 conservation laws:
$\frac{\partial \mathcal{L}}{\partial \dot{\phi}}=mr^2\dot{\phi}^2=mh$ which is a constant.
$$\mathcal{L}-\dot{r} \frac{\partial \mathcal{L}}{\partial \dot{r}}-\dot{\phi} \frac{\partial \mathcal{L}}{\partial \dot{\phi}}=c$$
and
$$m\left( \frac{\dot{r}^2}{2}+\frac{r^2\dot{\phi}^2}{2}+\frac{GM}{r}-\dot{r}-r^2\dot{\phi}^2 \right)=\dot{r}^2+\frac{h^2}{r^2}-\frac{2GM}{r}=E.$$
Define $u=\frac{1}{r}$.
$$\frac{du}{dr}=-\frac{1}{r^2}$$
$$\left( \frac{du}{d\phi} \right)^2=\left( \frac{du}{dr} \frac{dr}{d\phi} \right)^2=\frac{1}{r^4}\left( \frac{dr}{d\phi} \right)^2=\frac{1}{r^4}\left( \frac{\dot{r}^2}{\dot{\phi}^2} \right)=\frac{\dot{r}^2}{h}$$
$$\therefore\left( \frac{du}{d\phi} \right)^2=\frac{E}{h^2}-\frac{1}{r^2}+\frac{2GM}{rh^2}$$
$$\left( \frac{du}{d\phi} \right)^2+\left( u-\frac{GM}{h^2} \right)^2=\frac{E}{h^2}+\frac{G^2M^2}{h^4}.$$
This is solved by
$$u=u_{0}\left( \frac{GM}{h^2}+u_{1}\cos(\phi-\phi_{0}) \right)$$
s.t.
$$u_{0}^2u_{1}^2=\frac{E}{h^2}+\frac{G^2M^2}{h^4}.$$
There are 3 cases,
- $u_{1}=0$, this gives a constant radius so a circular orbit
- $u_{1}\in\left( 0,\frac{GM}{h^2} \right)$, this gives an elliptical orbit
- $u_{1}\geq \frac{GM}{h^2}\implies u\to 0\implies r\to \infty$ which is a scattering orbit.
