The aim is to integrate a complex function $f(z)$ along a path $\gamma$, $\int_{\gamma} f(z)dz$.
Using definition from of $f(z)$ from the [Cauchy-Riemann derivation](Complex%20Differentiation.md), we can rewrite this integral as
$$\int_{\gamma}f(z)dz=\int_{\gamma}(u(x,y)+iv(x,y))(dx+idy)=\int_{\gamma}(udx-vdy)+i\int_{\gamma}(vdx+udy).$$
Typically, $\gamma$ is parameterised in terms of $t\in\mathbb{R}$.

Another way to evaluate this integral if $a\leq t\leq b$ is
$$\int_{\gamma}f(z)dz=\int_{a}^b f(\gamma(t))\gamma'(t)dt.$$
### Example:
$$\int_{\gamma}z^2dz\text{ where $\gamma$ is the path that maps [0,$\pi$] to $\mathbb{C}$}.$$
##### Method 1:
$$f(z)=z^2=(x+iy)^2=(x^2-y^2)+i(2xy)$$
$$u(x,y)=x^2-y^2\text{ and } v(x,y)=2xy$$
Define $\gamma(t)=e^{it}$, which gives $x=\cos t$, and $y=\sin t$.
This gives
$$u(x,y)=x^2-y^2=\cos^2t-\sin^2t=\cos (2t)$$
$$v(x,y)=2\cos t\sin t=\sin(2t)$$
and $dx=-\sin(t)dt$ and $dy=\cos(t)dt$.
Compute integral:
$$\int_{\gamma}z^2dz=\int_{0}^\pi(udx-vdy)+i \int_{0}^\pi(vdx+udy)$$
$$=\int_{0}^\pi(-\cos(2t)\sin(t)-\sin(2t)\cos(t))dt+i\int_{0}^\pi(-\sin(2t)\sin(t)+\cos(2t)\cos(t))dt$$
$$=\int_{0}^\pi-\sin(3t)dt+i \int_{0}^\pi \cos(3t)dt=-\frac{2}{3}.$$
##### Method 2:
$\gamma(t)=e^{it}$; $\gamma'(t)=ie^{it}dt$. Plug into equation to solve integral:
$$\int_{\gamma}z^2dz=\int_{0}^\pi f(\gamma(t))\gamma'(t)dt=\int_{0}^\pi(e^{it})^2ie^{it}dt$$
$$=i \int_{0}^\pi e^{3it}dt=-\frac{2}{3}.$$
