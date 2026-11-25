Let $f$ be a [meromorphic](Laurent%20Series.md) function in domain $D$ with set of [poles](Poles%20and%20Zeros.md) $\{z_{i}\}$. A closed contour integral of $f(z)$ over a contour enclosing the singularities is given by
$$\oint_{C}f(z)dz=2\pi i\sum_{i}\text{Res}[f,z_{i}].$$
'Proof':
![[Pasted image 20241106102920.png]]
Consider a contour enclosing three poles. We shall shrink the contour so that it becomes 4 contours - 1 for each pole and one at the origin.
$$\oint_{C}f(z)dz=\left[\oint_{C_{1}}+\oint_{C_{2}}+\oint_{C_{3}}+\cancelto{0}{\oint_{C_{4}}}\right]f(z)dz.$$
As $f$ is analytic in the domain enclosed by the contour $C_{4}$, the closed integral over this contour is zero by [[Cauchy's theorem]].

This gives
$$\oint_{C}f(z)dz=\oint_{C_{1}}f(z)dz+\oint_{C_{2}}f(z)dz+\oint_{C_{3}}f(z)dz.$$
Each contour integral can be evaluated using the result from [[Integrating Meromorphic Functions]], which gives
$$\oint_{C}f(z)dz=2\pi i\text{Res}[f,z_{1}]+2\pi i\text{Res}[f,z_{2}]+2\pi i\text{Res}[f,z_{3}]=2\pi i\sum_{i=1}^3\text{Res}[f,z_{i}]$$
$$\square.$$
Example:
Evaluate
$$\oint_{C} \frac{\cos(\pi z)}{z^2(1-z)}dz$$
over the contours $C_{1}:\lvert z \rvert=\frac{1}{2}$, and $C_{2}:\lvert z \rvert=2$.

We can see the poles of this function are at $z=0$ of order 2 and a simple pole at $z=1$.
First [evaluate](Calculating%20Residues.md) the simple pole
$$\text{Res}[f,1]=\lim_{ z \to 1 }(z-1) \frac{\cos(\pi z)}{z^2(1-z)}=\lim_{ z \to 1 } -\frac{\cos(\pi z)}{z^2}= -\frac{\cos(\pi)}{1}=1$$
For the pole of order two, it may be easier to find the residue from the $a_{-1}$ coefficient in the [[Laurent Series]]:
$$\frac{\cos(\pi z)}{z^2(1-z)}=\frac{1}{1-z} \frac{\cos(\pi z)}{z^2}=\frac{1}{z^2}\sum_{n=0}^\infty z^n\sum_{m=0}^\infty \frac{(-1)^m}{m}(\pi z)^m$$
$$=\frac{1}{z^2}(1+z+z^2+\mathcal{O}(z^3))\left( 1-\frac{1}{2}(\pi z)^2+\mathcal{O}(z^4) \right)$$
$$=\frac{1}{z^2}+\frac{1}{z}+1+\dots-\frac{1}{2}\pi^2-\frac{1}{2}\pi^2z.$$
From this we can see that $a_{-1}=1$ so $\text{Res}[f,0]=1$
Using residue theorem we can now evaluate the integral. For $C_{1}$, only the pole at $z=0$ in enclosed by the contour so 
$$\oint_{C_{1}} \frac{\cos(\pi z)}{z^2(1-z)}dz=2\pi i.$$
For $C_{2}$, both poles are enclosed by the contour so 
$$\oint_{C_{2}} \frac{\cos(\pi z)}{z^2(1-z)}dz=2\pi i+2\pi i=4\pi i.$$
