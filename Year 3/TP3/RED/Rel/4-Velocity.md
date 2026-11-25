The [contravariant](Index%20and%20Tensor%20Notation.md) 4-vector for velocity is given by
$$u^\mu=\frac{dx^\mu}{d\tau}.$$
We used proper time instead of observer time for this as it yields a contravariant vector while observer time doesn't.
$$u'^\mu=\frac{dx'^\mu}{d\tau}=\frac{d(\Lambda^\mu_{\;\nu}x^\nu)}{d\tau}=\Lambda^\mu_{\;\nu} \frac{dx^\nu}{d\tau}=\Lambda^\mu_{\;\nu}u^\nu.$$
If we use observer time:
$$\frac{dx'^\mu}{dt'}=\frac{d(\Lambda^\mu_{\;\nu}x^\nu)}{dt'}=\Lambda^\mu_{\;\nu} \frac{dx^\nu}{d(\gamma t-\gamma \beta x/c)}\neq \Lambda^\mu_{{\;\nu}}u^\nu$$
so using observer time does not give us a contravariant vector.

Evaluating $u^\mu$:
$$u^\mu=\frac{dx^\mu}{d\tau}=\frac{dt}{d\tau} \frac{dx^\mu}{dt}=\gamma(v)\left( c \frac{dt}{dt}, \frac{dx}{dt}, \frac{dy}{dt}, \frac{dz}{dt} \right)=\gamma(v)(c,\underline{v}).$$
The covariant 4-velocity can be obtained using the metric
$$u_{\mu}=g_{\mu \nu}u^\nu=\gamma(c,-\underline{v}).$$
This can be used to calculate the Minkowski norm
$$u^\mu u_{\mu}=\gamma^2(c^2-v^2)$$
In the rest frame $v=0$, $\gamma=1$ so $u^\mu u_{\mu}=c^2$ in all reference frames.