If $f(z)$ is analytic on a [simply connected](Curves%20and%20Simply%20Connected%20Regions.md) domain $D$ that is contained by closed curve $C$ with $a\in D$ then
$$f(a)=\frac{1}{2\pi i}\oint_{C} \frac{f(z)}{z-a}dz.$$
Example:
Evaluate
$$\oint_{C} \frac{z}{z^2+1}dz$$
along the curve $C:|z-i|=\frac{1}{2}$.
$$\oint_{C} \frac{z}{z^2+1}dz=\oint_{C} \frac{z}{(z+i)(z-i)}dz.$$
This integral has two singularities, $z=\pm i$. Only $z=i$ is inside the region enclosed by $C$ so $a=i$ and $f(z)=\frac{z}{z+i}$.
Using Cauchy's integral formula:
$$f(a)=f(i)=\frac{i}{i+i}=\frac{1}{2}$$
$$\therefore \oint_{C} \frac{z}{z^2+1}dz=2\pi if(i)=\pi i.$$
