The gamma function extends the definition of the factorial for non-integer values.
It appears in integrals and ODEs in QFT, thermodynamics,$\dots$
In thermodynamics, the number of particles is given by
$$N=\int_{0}^{\infty}g(E)f(E)dE=\int_{0}^{\infty}E^{1/2}e^{ -E/k_{B}T }.$$
The gamma function is defined by
$$\Gamma(x)=\int_{0}^{\infty }t^{x-1}e^{ -t }dt.$$
If $x$ is a positive integer then this reduces to a factorial,
$$\Gamma(n)=(n-1)!.$$
Recursive property:
$$\Gamma(x+1)=\int_{0}^{\infty}t^{x}e^{ -t }=\cancelto{0}{[-t^{x}e^{ -t }]_{0}^{\infty}}+\int_{0}^{\infty}xt^{x-1}e^{ -t }dt=x \int_{0}^{\infty}t^{x-1}e^{ -t }dt$$
$$\Gamma(x+1)=x\Gamma(x).$$
Proof of the factorial property by induction:
$$\Gamma(1)=\int_{0}^{\infty}dtt^{0}e^{ -t }=[-e^{ -t }]_{0}^{\infty}=1$$
$$\Gamma(2)=1\Gamma(1)=1$$
$$\Gamma(3)=2\Gamma(2)=2$$
$$\Gamma(4)=3\Gamma(3)=6$$
$$\implies\Gamma(n)=(n-1)\Gamma(n-1)=(n-1)(n-2)\Gamma(n-2)=(n-1)!\;\square$$
For small $x$,
$$\Gamma(x)=\frac{\Gamma(x+1)}{x}\approx \frac{1}{x}.$$
For non-integer $x$:
$$\Gamma\left( \frac{1}{2} \right)=\int_{0}^{\infty}dtt^{-1/2}e^{ -t }$$
Let $u=\sqrt{ t }$, $dt=2udu$,
$$=\int_{0}^{\infty}2udu \left( \frac{1}{u} \right)e^{ -u^2 }=2\int_{0}^{\infty}due^{ -u^2 }=\frac{2\sqrt{ \pi }}{2}=\sqrt{ \pi }.$$
For negative $x$, the definition is extended using the recursive property:
$$-\frac{1}{2}\Gamma\left( -\frac{1}{2} \right)=\Gamma\left( \frac{1}{2} \right)=\sqrt{ \pi }\implies\Gamma\left( -\frac{1}{2} \right)=2\sqrt{ \pi }.$$

The Beta function is defined as
$$B(u,v)=\int_{0}^{1}dtt^{u-1}(1-t)^{v-1}$$
where
$$\begin{cases}
\mathrm{Re}(u)>0 \\
\mathrm{Re}(v)>0
\end{cases}.$$
$$B(u,v)=B(v,u).$$
Consider $\Gamma(u)\Gamma(v)$:
$$\Gamma(u)\Gamma(v)=\int_{0}^{\infty}e^{ -t }t^{u-1}dt \int_{0}^{\infty}e^{ -s }s^{v-1}ds=\int_{0}^{\infty}dt\int_{0}^{\infty}dse^{ -(t+s) }t^{u-1}s^{v-1}.$$
Let $x=s+t$, $t=xy$, $s=x(1-y)$.
Form the [Jacobian](Coordinate%20Changes.md)
$$J=\begin{vmatrix}
y & x \\
1-y & -x
\end{vmatrix}=|-yx-(1-y)x|=|-x|=|x|.$$
$$\Gamma(u)\Gamma(v)=\int_{0}^{\infty}xdx \int_{0}^{1}dye^{ -x }x^{u-1}y^{u-1}x^{v-1}(1-y)^{v-1}=\Gamma(u+v)B(u,v)$$
$$\implies B(u,v)= \frac{\Gamma(u)\Gamma(v)}{\Gamma(u+v)}.$$
Change of coordinates:
$$t=\cos^2\phi$$
$$dt=-2\cos \phi \sin \phi d\phi.$$
$t=0\implies \phi=\frac{\pi}{2}$ and $t=1\implies \phi=0$
$$B(u,v)=-2\int_{\frac{\pi}{2}}^{0}(\cos \phi)^{2u-2}(\sin \phi)^{2v-2}\cos \phi \sin \phi d\phi$$
$$=2\int_{0}^{\pi/2} d\phi(\cos \phi)^{2u-1}(\sin \phi)^{2v-1}.$$
