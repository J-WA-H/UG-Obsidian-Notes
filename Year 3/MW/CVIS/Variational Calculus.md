Variational calculus defines how something changes under perturbations.
This is based on the Taylor expansion,
$$f(x+\delta t)=\sum_{n=0}^{\infty} \frac{1}{n!}f^{(n)}(t)\delta t^{n}.$$
The definition of a derivative is
$$\frac{df}{dt}=\lim_{ \delta t \to 0 } \frac{{f(t+\delta t)-f(t)}}{\delta t}.$$
Example: $\sin(t+\delta t)=\sin(t)+\cos(t)\delta t-\frac{1}{2}\sin(t)\delta t+\dots$.
$$\frac{d\sin(t)}{dt}=\lim_{ \delta t \to 0 } \frac{{\sin(t+\delta t)-\sin(t)}}{\delta t}=\lim_{ \delta t \to 0 } \frac{{\cos(t)\delta t-\frac{1}{2}\sin(t)\delta t^2+\mathcal{O}(\delta t^3)}}{\delta t}=\cos(t).$$
Sometimes it is useful to approximate at finite $\delta t$,
$$\frac{df}{dt}\approx \frac{{f(t+\delta t)-f(t)}}{\delta t}$$
where
$$f(t+\delta t)=f(t)+\frac{df}{dt}\delta t+R(r,\delta t)$$
with the remainder
$$R(t,\delta t)=\sum_{n=2}^{\infty} \frac{\delta t^nf^{(n)}(t)}{n!}.$$
Consider
$$\frac{R}{\delta t}=\delta t \frac{f''}{2!}+\dots$$
so as $\delta t\to{0}$, $\frac{R}{\delta t}\to 0$ s.t. $\frac{R}{\delta t}=\mathcal{O}(\delta t)$.
However, 
$$\frac{R}{\delta t^2}=\frac{f''}{2!}+\dots$$
so as $\delta t\to 0$, $\frac{R}{\delta t}\to \frac{f''}{2!}$. If $f$ is analytic then $f''$ is well defined.
$$R=\mathcal{O}(\delta t^2).$$
