Definition: Let $f$ be analytic on a  [simply connected](Curves%20and%20Simply%20Connected%20Regions.md) domain $D$, then $\forall \;z_{0}\in D$ $\exists$ a radius $r$ s.t. $|z-z_{0}|<r$, then its Taylor series is defined by
$$f(z)=\sum_{n=0}^\infty \frac{f^{(n)}(z_{0})}{n!}(z-z_{0})^n.$$
Proof:
This will make use of the identity $$\frac{1}{1-\varepsilon}\equiv \sum_{n=0}^\infty \varepsilon^n\text{ where }|\varepsilon|<1.$$
Using [Cauchy's formula](Derivatives%20with%20Cauchy's%20Formula.md) and $\zeta \in \mathbb{C}$:
$$f^{(n)}(z_{0})=\frac{n!}{2\pi i}\oint_{C} \frac{f(\zeta)}{(\zeta-z_{0})^{n+1}}d\zeta.$$
Divide through be $\frac{n!}{(z-z_{0})^n}$:
$$\frac{f^{(n)}(z_{0})(z-z_{0})^n}{n!}=\frac{1}{2\pi i}\oint_{C} \frac{f(\zeta)(z-z_{0})^n}{(\zeta-z_{0})^n}d\zeta.$$
Take sum of both sides:
$$\sum_{n=0}^\infty \frac{f^{(n)}(z_{0})}{n!}(z-z_{0})^n=\sum_{n=0}^\infty \frac{1}{2\pi i}\oint_{C} \frac{f(\zeta)(z-z_{0})^n}{(\zeta-z_{0})^{n+1}}d\zeta$$
$$=\frac{1}{2\pi i} \oint_{C} \sum_{n=0}^\infty \frac{f(\zeta)}{(\zeta-z_{0})}\left( \frac{{z-z_{0}}}{\zeta-z_{0}} \right)^nd\zeta.$$
as $\zeta>z$ , $\left( \frac{{z-z_{0}}}{\zeta-z_{0}} \right)<1$
$$\therefore \sum_{n=0}^\infty\left( \frac{{z-z_{0}}}{\zeta-z_{0}} \right)^n=\frac{1}{1-\left( \frac{{z-z_{0}}}{\zeta-z_{0}} \right)}=\frac{{\zeta-z_{0}}}{\zeta-z}$$
$$\implies \frac{1}{2\pi i} \oint_{C} \sum_{n=0}^\infty \frac{f(\zeta)}{(\zeta-z_{0})}\left( \frac{{z-z_{0}}}{\zeta-z_{0}} \right)^nd\zeta=\frac{1}{2\pi i}\oint_{C} \frac{f(\zeta)}{(\zeta-z_{0})}\left( \frac{{\zeta-z_{0}}}{\zeta-z} \right)d\zeta$$
$$=\frac{1}{2\pi i}\oint_{C} \frac{f(\zeta)}{\zeta-z}d\zeta=f(z)$$
$$\therefore f(z)=\sum_{n=0}^\infty \frac{f^{(n)}(z_{0})}{n!}(z-z_{0})^n.$$
