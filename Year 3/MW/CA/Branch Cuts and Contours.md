If the integrand contains a [branch point](Complex%20Functions%20and%20Branch%20Points.md), which makes it multivalued. To make this analytic a branch cut must be made. Because of this branch cut, we need to be careful about the contour we choose as it can pass through the branch cut.
![[Pasted image 20241107153901.png]]
For example, the complex logarithm has a branch point at the origin so the above branch cut is made. When integrating, we use the contour above.

Example:
$$I=\int_{0}^{\infty} \frac{u^{-y}}{1+u}du;\;y\in(0,1).$$
Complexifying the integral gives
$$I=\oint_{C} \frac{z^{-y}}{1+z}dz;\;y\in(0,1).$$

$$f(z)=\frac{z^{-y}}{1+z};\;z^{-y}=\exp[-y\ln z].$$
At large $z$, $\lvert z \rvert\to C_{R}$ so $\lvert z \rvert\approx R$
$$f(z)=\frac{R^{-y}}{1+R}\approx R^{-(y+1)}.$$
as $1<y+1<2$, $f(z)$ is [vanishing](Evaluating%20Real%20Integrals.md) so the integral over $C_{R}$ disappears.

At small $z$, $\lvert z \rvert=\varepsilon$ so
$$f(z)=\frac{\varepsilon^{-y}}{1+\varepsilon}\approx\varepsilon^{-y}.$$
$z=\varepsilon e^{i\theta}$, $d\theta=i\varepsilon e^{i\theta}$
$$\therefore \left\lvert  \oint_{C_{\varepsilon}}f(z)dz \right\rvert <\lvert \varepsilon^{-y}i\varepsilon e^{i\theta} \rvert = \lvert \varepsilon^{1-y} \rvert\to {0}.$$
This leaves the only non-zero contributions are the contours $I$, $I'$.
For $I$, $z=x+i\varepsilon$, and for $I'$, $z=x-i\varepsilon$.
$$\oint_{C}f(z)dz=\oint_{I}f(z)dz+\oint_{I'}f(z)dz$$
$$=\int_{0}^{\infty}f(x+i\varepsilon)dx+\int_{0}^{\infty}f(x-i\varepsilon)dx.$$
$$f(x+i\varepsilon)-f(x-i\varepsilon)=\frac{(R'e^{i\varepsilon/x})^{-y}}{1+R'e^{i\varepsilon/x}}-\frac{(R'e^{i(2\pi-\varepsilon/x)})^{-y}}{1+R'e^{i(2\pi-\varepsilon/x)}}.$$
$$=\frac{R'^{-y}(1-e^{-i{2}\pi y})}{1+R'}$$
$\varepsilon\to{0}\implies R'=x$
$$\implies \int_{0}^{\infty}dx[f(x+i\varepsilon)-f(x-i\varepsilon)]=(1-e^{-i{2}\pi y})\int_{0}^{\infty} \frac{x^{-y}}{1+x}dx$$
$$\therefore \int_{0}^{\infty} \frac{x^{-y}}{1+x}dx=\frac{1}{1-e^{-i 2\pi y}}\oint_{C}f(z)dz=\frac{2\pi i}{1-e^{-i 2\pi y}}\sum_{i}\text{Res}[f,z_{i}].$$
The extra factor from using [[Residue Theorem]] comes from the fact there is a branch point.

The only pole of this function is $z=-1$:
$$\text{Res}[f,-1]=\lim_{ z \to -1 }(z+1) \frac{z^{-y}}{1+z}=\lim_{ z \to -1 } z^{-y}=(-1)^{-y}=e^{-i\pi y}.$$
$$\therefore I=\frac{2\pi ie^{-i\pi y}}{e^{-i\pi y}(e^{i\pi y}-e^{-i\pi y})}=\frac{\pi}{\sin(\pi y)}.$$
