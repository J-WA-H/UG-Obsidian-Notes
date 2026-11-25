Let $f$ be a [meromorphic](Laurent%20Series.md) function inside a closed curve $C$, 
$$\frac{1}{2\pi i}\oint_{C} \frac{f'(z)}{f(z)}dz=n_{zeros}-n_{poles}$$
where $n_{poles}$ and $n_{zeros}$ are the numbers of [[Poles and Zeros]] respectively.
Proof:
If $f$ has a pole at $z_{0}$ then $f'$ also has a pole at $z_{0}$ that is one order higher.
$\implies \frac{f'(z)}{f(z)}$ has a simple pole.

If $f$ has a zero at $z_{0}$, $f(z)=(z-z_{0})g(z)$, where $g$ is analytic and $g(z_{0})\neq 0$.
$$\frac{f'(z)}{f(z)}=\frac{{n(z-z_{0})^{\cancel{n-1}}g(z)+\cancel{(z-z_{0})^n}g'(z)}}{\cancel{(z-z_{0})^n}g(z)}$$
$$=\frac{n}{z-z_{0}}+\frac{g'(z)}{g(z)}.$$
$$\therefore \oint_{C} \frac{f'(z)}{f(z)}dz=\oint_{C} \frac{n}{z-z_{0}}+\cancelto{0}{\oint_{C} \frac{g'(z)}{g(z)}dz}.$$
The second term goes to zero from [[Cauchy's theorem]] as $g$, $g'$ are analytic. 
$$\therefore \oint_{C} \frac{f'(z)}{f(z)}dz=\oint_{C} \frac{n}{z-z_{0}}dz=2\pi in.$$
This integral was evaluated using [[Cauchy's Integral Formula]].
So only considering zeros:
$$\frac{1}{2\pi i}\oint_{C} \frac{f'(z)}{f(z)}dz=n_{zeros}.$$
Now considering poles:
Take $f(z)=\frac{g(z)}{(z-z_{0})^m}$:
$$f'(z)=\frac{{(z-z_{0})^mg'(z)-m(z-z_{0})^{m-1}g(z)}}{(z-z_{0})^{2m}}$$
$$\frac{f'(z)}{f(z)}=\frac{{(z-z_{0})^m[(z-z_{0})^mg'(z)-m(z-z_{0})^{m-1}g(z)]}}{(z-z_{0})^{2m}g(z)}=\frac{g'(z)}{g(z)}-\frac{m}{(z-z_{0})^{m+1}}.$$
$$\oint_{C} \frac{f'(z)}{f(z)}dz=\cancelto{0}{\oint_{C} \frac{g'(z)}{g(z)}dz}-\oint_{C} \frac{m}{(z-z_{0})^{m+1}}dz.$$
Using [[Derivatives with Cauchy's Formula]], we get
$$\oint_{C} \frac{f'(z)}{f(z)}dz=-2\pi im.$$
So considering a function with $n$ zeros and $m$ poles we have
$$\frac{1}{2\pi i}\oint_{C} \frac{f'(z)}{f(z)}dz=n-m$$
$$\square$$
