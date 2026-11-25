Let $D\subset\mathbb{C}$ be a simply connected [open subset](Complex%20Differentiation.md) in $\mathbb{C}$ and let $f$ be [analytic](Complex%20Differentiation.md) in $D$, then $f:D\to\mathbb{C}$. For any closed curve in $D$:
$$\oint_{C}f(z)dz=0.$$
![[Pasted image 20241015145910.png]]
###### Justification (vague proof):
Recall Green's theorem:
$$\oint_{C}[Adx+Bdy]=\iint_{S}\left[ \frac{\partial B}{\partial x}-\frac{\partial A}{\partial y} \right]dxdy$$
Green's theorem transforms a line integral around $C$ into a double integral over the region $S$ inside $C$. We note that $S$ spans $C$. From definitions of [complex functions](Complex%20Differentiation.md),
$$\oint_{C}f(z)dz=\oint_{C}(udx-vdy)+i\oint_{C}(vdx+udy)$$
$$=\iint_{S}\left[ \frac{\partial}{\partial x}(-v+iu)-\frac{\partial}{\partial y}(u+iv) \right]dxdy$$
$$=\iint_{S}\left[ -\frac{\partial v}{\partial x}-\frac{\partial u}{\partial y} +i\left( \frac{\partial u}{\partial x}-\frac{\partial v}{\partial y} \right)\right]=0\text{ from Cauchy Riemann equations}$$
##### Corollaries of Cauchy's theorem
- Let $\gamma_{1}$ and $\gamma_{2}$ be two curves from $z_1$ to $z_2$ where $f(z)$ is analytic on a [simply connected](Curves%20and%20Simply%20Connected%20Regions.md) domain containing $z_1$ and $z_2$, then:
	$$\int_{\gamma_{1}}f(z)dz=\int_{\gamma_{2}}f(z)dz$$
	##### Proof:
	Let $C=\gamma_{1}-\gamma_{2}$, i.e. a closed curve. By Cauchy's theorem, we have
	$$\oint_{C}f(z)dz=0\text{ so } \int_{\gamma_{1}}f(z)dz-\int_{\gamma_{2}}f(z)dz=0$$
	$$\implies \int_{\gamma_{1}}f(z)dz=\int_{\gamma_{2}}f(z)dz.$$
- Let $C_1$ and $C_2$ be closed contours enclosing simply connected domains $D_1$ and $D_2$, and let $f(z)$ be analytic on $D=D_1-D_2$, then
	$$\oint_{C_{1}}f(z)dz=\oint_{C_{2}}f(z)dz$$
	#### Proof:
	![[Pasted image 20241015150941.png]]
	Let $C$ be the curve following the outline of the shape in the bottom right region.
	$$C=C_2-AB+\gamma_{AB}-(C_{1}-BC)+\gamma_{CD}$$
	$$\oint_{C}f(z)dz=\oint_{C_{2}}f(z)dz-\int_{A}^Df(z)dz+\int_{A}^Bf(z)dz-\oint_{C_{2}}f(z)dz+\int_{B}^Cf(z)dz+\int_{C}^Df(z)dz$$
	This expression is equal to 0 due to Cauchy's theorem.
	$$0=\oint_{C_{2}}f(z)dz-\oint_{C_{1}}f(z)dz+\cancelto{0}{\left[ \int_{A}^B +\int_{B}^C+\int_{C}^D+\int_{D}^A \right]f(z)dz}.$$
	As the square brackets show a closed curve in a rectangle, due to Cauchy's theorem it goes to zero.
	$$\therefore \oint_{C_{1}}f(z)dz=\oint_{C_{2}}f(z)dz$$
	This corollary is useful when we are integrating around a complicated contour, as we can deform it into a more convenient curve.