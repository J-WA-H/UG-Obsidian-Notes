Consider a continuous, differentiable surface that can be described by a metric.

For $ds^2>0$ $\forall$ $x$, this is a Riemannian surface. The universe is pseudo-Riemannian. Using [[Curvature as Distance]],
![[Pasted image 20260130094659.png]]
The metric encodes real curvature, a fundamental quantity, done in coordinates, not fundamental.

Consider two tangent vectors to the function $\vec{\lambda}(s)$.
![[Pasted image 20260130095634.png]]
To work out the derivative of this function, slide the vectors so the tails touch so we can compare, allowing differentiation,
![[Pasted image 20260130095801.png]]
Sliding vectors doesn't work on a curved surface so differentiation causes problems.
$$\vec{\lambda}=\lambda^a(s)\vec{e}_{a}\tag{4.1} .$$The path length is denoted by $s$. Try
$$\frac{d\lambda^\bar{a}}{ds}=\lim_{ \delta s \to 0 } \frac{{\lambda^a(s+\delta s)-\lambda^a(s)}}{\delta s}.\tag{4.2} $$
Using the transformation for a [contravariant tensor](Tensors%20and%20Metrics.md),
$$\frac{d\lambda^\bar{a}}{ds}=\frac{d}{ds}\left( \frac{\partial x^\bar{a}}{\partial x^b}\lambda^b \right)=\frac{\partial x^\bar{a}}{\partial x^b} \frac{d\lambda^b}{ds}+\frac{d}{ds}\left( \frac{\partial x^\bar{a}}{\partial x^b} \right)\lambda^b\tag{4.3} .$$This shows that $\frac{d\lambda^a}{ds}$ does not transform as a tensor. The extra term comes from the fact that the vectors are at different points $\vec{\lambda}=\lambda^a\vec{e}_{a}$. If the only action is sliding, the length and direction is unchanged. These are the parallel transport conditions.
$$\therefore \frac{d\lambda_{\parallel}}{ds}=0=\frac{d}{ds}(\lambda^a\vec{e}_{a})=\frac{d\lambda^a}{ds}\vec{e}_{a}+\lambda^a \frac{d\vec{e}_{a}}{ds}\tag{4.4}. $$This shows the basis vector changes with position.
$$=\frac{d\lambda^a}{ds}\vec{e}_{a}+\lambda^a \frac{\partial \vec{e}_{a}}{\partial x^b}\left( \frac{dx^b}{ds} \right).\tag{4.5} $$
We define
$$\frac{\partial \vec{e}_{a}}{\partial x^b}=\Gamma^c_{\;ab}\vec{e}_{c}\tag{4.6} $$where $\Gamma^c_{\;ab}$ is the Christoffel symbol, which is not a tensor.
$$\therefore \frac{d\vec{\lambda}}{ds}=\frac{d\lambda^a}{ds}\vec{e}_{a}+\lambda^a\Gamma^c_{\;ab}\vec{e}_{c} \frac{dx^b}{ds}\tag{4.7} .$$Shift indices,
$$\frac{d\vec{\lambda}}{ds}=\frac{d\lambda^a}{ds}\vec{e}_{a}+\lambda^b\Gamma^a_{\;bc}\vec{e}_{a} \frac{dx^c}{ds}=\left( \frac{d\lambda^a}{ds}+\Gamma^a_{\;bc}\lambda^b \frac{dx^c}{ds} \right)\vec{e}_{a}.\tag{4.8} $$
Using the parallel transport condition,
$$\frac{d\lambda_{\parallel}}{ds}+\Gamma^a_{\;bc}\lambda_{\parallel}^b \frac{dx^c}{ds}=0\tag{4.9}. $$
This gives
$$\frac{\delta\lambda^a}{\delta s}=-\Gamma^a_{\;bc}\lambda^b_{\parallel} \frac{\delta x^c}{\delta s}\implies\delta\lambda^a=-\Gamma^a_{\;bc}\lambda_{\parallel}^b\delta x^c\tag{4.10}. $$
This gives the parallel transport vector
$$\lambda_{\parallel}(s+\delta s)=\lambda^a(s)+\delta\lambda^a_{\parallel}=\lambda^a(s)-\Gamma^a_{\;bc}\lambda^b\delta x^c.\tag{4.11} $$
From this
$$\frac{{\vec{\lambda}(s+\delta s)-\vec{\lambda}_{\parallel}(s+\delta s)}}{\delta s}\tag{4.12} $$gives the real physics such as direction and magnitude have changed.
$$\frac{{\left( \lambda^a(s)+\frac{d\lambda^a}{ds}\delta s \right)-(\lambda^a(s)-\Gamma^a_{\;bc}\lambda^b\delta x^c)}}{\delta s}=\frac{d\lambda^a}{ds}+\Gamma^a_{\;bc}\lambda^b \frac{\delta x^c}{\delta s}=\frac{D\lambda^a}{ds}.\tag{4.13} $$The terms that make each term not a tensor not a tensor exactly cancel so the whole thing is a tensor. The absolute derivative is defined as
$$\frac{D\lambda^a}{ds}=\frac{d\lambda^a}{ds}+\Gamma^a_{\;bc}\lambda^b \frac{dx^c}{ds}\tag{4.14}. $$
If $\frac{D\lambda^a}{ds}=0$, this is parallel transport so no physics happens.
If $\frac{D\lambda^a}{ds}\neq 0$, physics happens from some imposed force.

Using a path $s(x^c)$,
$$\frac{D\lambda^a}{ds}=\frac{\partial\lambda^a}{\partial x^c} \frac{dx^c}{ds}+\Gamma^a_{\;bc}\lambda^b \frac{dx^c}{ds}=\left( \frac{\partial x^a}{\partial x^c}+\Gamma^a_{\;bc}\lambda^b \right) \frac{dx^c}{ds}\tag{4.15} =\lambda^a_{\;;c} \frac{dx^c}{ds}.$$This defines the covariant derivative, useful as it is not dependent on the choice of path,
$$\lambda^a_{\;;c}=\frac{\partial\lambda^a}{\partial x^c}+\Gamma^a_{\;bc}\lambda^b\tag{4.16}. $$
