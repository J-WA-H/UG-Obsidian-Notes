We can use all the techniques for integrating in the complex plane to evaluate real integrals that can't be solved using real analysis methods - one example being trigonometric integrals,
$$I=\int_{0}^{2\pi}d\theta R(\cos (m\theta),\sin(n\theta)).$$
We aim to generalise this integral in the complex plane, so we will call $z=e^{i\theta}$; $\theta\in[0,2\pi]$.
From this we get
$$dz=ie^{i\theta}d\theta \implies d\theta=\frac{dz}{iz}.$$
This moves the integral from
$$\int_{0}^{2\pi}d\theta=\oint_{C} \frac{dz}{iz}$$
where $C$ is the unit circle in the $\mathbb{C}$ plane.
The trig functions can also be rewritten in terms of $z$:
$$\cos(m\theta)=\frac{{e^{im\theta}+e^{-im\theta}}}{2}=\frac{{z^{m}+z^{-m}}}{2}$$
$$\sin(n\theta)=\frac{{e^{in \theta}-e^{-in \theta}}}{2i}=\frac{{z^{n}-z^{-n}}}{2i}.$$
Example:
$$I=\int_{0}^{2\pi}d\theta\frac{\sin\theta}{(3+\cos \theta)(2+\sin \theta)}$$
Complexify the integral using $z=e^{i\theta}$:
$$I=\oint_{C} \frac{\left( \frac{{z-z^{-1}}}{2i} \right)}{\left( 3+\frac{{z+z^{-1}}}{2} \right)\left( 2+\frac{{z-z^{-1}}}{2i} \right)} \frac{dz}{iz}$$
$$=\oint_{C} dz \frac{z-z^{-1}}{z(6+z+z^{-1}) \frac{1}{2i}(4i+z-z^{-1})}=\oint_{C}dz \frac{-2i(z-z^{-1})}{(6z+z^2+1)(4i+z-z^{-1})}\cdot \frac{z}{z}$$
$$=\oint_{C}dz \frac{-2i(z^2-1)}{(6z+z^2+1)(4iz+z^2-1)}.$$
Find poles of this function and use [[Residue Theorem]] to evaluate the integral.
$$z^2+6z+1=0\implies z=-3\pm {2}\sqrt{ 2 }$$
$$z^2+4iz-1=0\implies z=(-2\pm \sqrt{ 3 })i.$$
As $C$ is the unit circle, only the poles at $z=-3+ 2\sqrt{ 2 }$ and $z=(-2+\sqrt{ 3 })i$ are relevant as they lie in the domain enclosed by $C$.
Now [calculate residues](Calculating%20Residues.md):
These are simple poles so can use limit definition so $\text{Res}[f,-3+2\sqrt{ 2 }]$ is given by
$$\lim_{ z \to -3+2\sqrt{ 2 } }(z-(-3+2\sqrt{ 2 })) \frac{{-2i(z^2-1)}}{(z-(-3+2\sqrt{ 2 }))(z-(-3-2\sqrt{ 2 }))(z-(-2i+\sqrt{ 3 }i))(z-(-2i+\sqrt{ 3 }i))}$$
$$=\lim_{ z \to -3+2\sqrt{ 2 } } \frac{{-2i(z^2-1)}}{(z-(-3-2\sqrt{ 2 }))(z-(-2i+\sqrt{ 3 }i))(z-(-2i+\sqrt{ 3 }i))}$$
$$=\frac{{-2i(16-12\sqrt{ 2 })}}{(4\sqrt{ 2 })(-3+2\sqrt{ 2 }+2i+i\sqrt{ 3 })(-3+2\sqrt{ 2 }+2i-i\sqrt{ 3 })}$$
$$= \frac{-2i 4\sqrt{ 2 }(-3+2\sqrt{ 2 })}{(4\sqrt{ 2 })(17-12\sqrt{ 2 }-6i-3i\sqrt{ 3 }+4i\sqrt{ 2 }+2i\sqrt{ 6 }-6i+4i\sqrt{2 }+3i\sqrt{ 3 }-2i\sqrt{ 6 }-4+2\sqrt{ 3 }-2\sqrt{ 3 }+3)}$$
$$=\frac{{-2i(-3+2\sqrt{ 2 })}}{(16-12\sqrt{ 2 }+(-12+8\sqrt{2})i)}=\frac{{-2i(-3+2\sqrt{ 2 })}}{(-3+2\sqrt{ 2 })(4\sqrt{ 2 }+4i)}$$
$$=-\frac{2i}{4\sqrt{ 2 }+4i}\cdot \frac{{\sqrt{ 2 }-i}}{\sqrt{ 2 }-i}=\frac{{-2i(\sqrt{ 2 }-i)}}{12}=-\frac{i(\sqrt{ 2 }-1)}{6}.$$
Now the other residue
$$\text{Res}[f,-2i+\sqrt{ 3 }i]=\lim_{ z \to -2i+\sqrt{ 3 }i } -\frac{2i(z^2-1)}{(z^2+6z+1)(z-(-2i-\sqrt{ 3 }i))}$$
$$=-\frac{2i(-8+4\sqrt{ 3 })}{(4\sqrt{ 3 }+(-12+6\sqrt{ 3 })i)(2\sqrt{ 3 }i)}=-\frac{2i(-8+4\sqrt{ 3 })}{-36+24\sqrt{ 3 }+24i}$$
$$=-\frac{8i(-2+\sqrt{ 3 })}{12(-3+2\sqrt{ 3 }+2i)}\cdot \frac{{-3+2\sqrt{ 3 }-2i}}{-3+2\sqrt{ 3 }-2i}$$
$$=\frac{-8i(12-7\sqrt{ 3 }+(4-2\sqrt{ 3 })i)}{12(25-12\sqrt{ 3 })}$$
$$=\frac{i(\sqrt{ 3 }-i)}{6}$$
so $$\oint_{C}f(z)dz=2\pi i\left(  \frac{i(\sqrt{ 3 }-i)}{6}-\frac{i(\sqrt{ 2 }-i)}{6} \right)=2\pi i\left(  \frac{i(\sqrt{ 3 }-\sqrt{ 2 })}{6} \right)=-\frac{\pi(\sqrt{ 3 }-\sqrt{ 2 })}{3}.$$
Note that as we are evaluating a real integral so the answer must be real.