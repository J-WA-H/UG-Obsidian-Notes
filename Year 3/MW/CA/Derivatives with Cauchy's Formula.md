6Differentiating [Cauchy's formula](Cauchy's%20Integral%20Formula.md) with respect to $a$ $n$ times gives
$$\frac{d^nf}{da^n}=\frac{n!}{2\pi i}\oint_{C} \frac{f(z)}{(z-a)^{n+1}}dz.$$
Proof for n=1 case:
$$\frac{df}{da}=\lim_{ \Delta a \to 0} \frac{f(a+\Delta a)-f(a)}{\Delta a}.$$
Apply Cauchy's formula to numerator:
$$f(a+\Delta a)=\frac{1}{2\pi i}\oint_{C} \frac{f(z)}{z-(a+\Delta a)}dz$$
$$f(a)=\frac{1}{2\pi i}\oint_{C} \frac{f(z)}{z-a}dz.$$
$$\frac{df}{da}=\lim_{ \Delta a \to 0 } \frac{1}{2\pi i\Delta a}\oint_{C} \frac{f(z)(z-a)-f(z)(z-a-\Delta a)}{[z-(a+\Delta a)][z-a]}dz$$$$=\lim_{ \Delta a \to 0 } \frac{1}{2\pi i\Delta a}\oint_{C} \frac{f(z)\Delta a}{[(z-a)^2-\Delta a(z-a)]}dz=\lim_{ \Delta a \to 0 } \frac{1}{2\pi i} \oint_{C} \frac{f(z)}{[(z-a)^2-\Delta a(z-a)]}dz$$
$$=\frac{1}{2\pi i}\oint_{C} \frac{f(z)}{(z-a)^2}dz$$
Further cases can be proved by induction (see workshop 4).

Example:
Evaluate
$$\oint_{C} \frac{{z+1}}{z^4+2z^3}dz$$
where $C:|z|=1$
$$\oint_{C} \frac{{z+1}}{z^4+2z^3}dz=\oint_{C} \frac{{z+1}}{z^3(z+2)}dz$$
The only singularity in the region enclosed by $C$ is $z=0$ so $a=0$ and
$$f(z)=\frac{{z+1}}{z+2}\implies \oint_{C} \frac{{z+1}}{z^4+2z^3}dz=\oint_{C} \frac{f(z)}{z^3}.$$
Using Cauchy's derivative formula, we can see that $n+1=3\implies n=2$.
$$\oint_{C} \frac{{z+1}}{z^3(z+2)}dz=f''(a)\cdot \frac{2\pi i}{n!}=\pi if''(a).$$
$$f'(z)=\frac{1}{(z+2)^2}\implies f''(z)=-\frac{2}{(z+2)^3}.$$
$$f''(0)=-\frac{2}{2^3}=-\frac{2}{8}=-\frac{1}{4}$$
$$\therefore \oint_{C} \frac{{z+1}}{z^4+2z^3}dz=-\frac{\pi i}{4}.$$
