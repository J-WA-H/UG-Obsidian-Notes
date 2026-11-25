Continuity: f is continuous if :
$$\lim_{ z \to z_{0} } f(z)=f(z_{0}) \iff \forall\; \varepsilon>0 \;\exists\;\delta>0 \text{ s.t. }|z-z_{0}|<\delta \implies|f(z)-f(z_{0})|<\varepsilon$$
### Differentiation in $\mathbb{C}$ plane:
We can consider differentiation in the $\mathbb{C}$ plane by extending the real case:
$$f'(z)=\lim_{ \delta \to 0 } \frac{{f(z+\delta)-f(z)}}{\delta}$$
which works for cases like $f(z)=z$ and $f(z)=z^2$.

However, using this limit for $f(z)=\bar{z}$, this gives $f'(z)=e^{-2i\theta}$, which depends on the direction you approach from, so even though the limit exists, this function is not differentiable.

#### Analytic functions
Definition: A neighbourhood of $z \in\mathbb{C}$ is an open set $U$ s.t. $z\in U$.
An open set is defined as a region in $\mathbb{C}$ that does not include its boundaries

Definition: A function is analytic/holomorphic if $\exists$ a neighbourhood $U$ of $z_{0}$ on which f is differentiable at all points in $U$.

Definition: A function is entire if it is differentiable on the whole complex plane.

#### Cauchy-Riemann Equations
We can now use these definitions to derive conditions for a function to be differentiable - that it must be the same no matter what direction you approach from.
Consider the function $f(z)=u(x,y)+iv(x.y)$ where $u$, $v$ are real functions.
$$f'(z_{0})=\frac{{f(z)-f(z_{0})}}{\delta}=\frac{{u(x_{0}+\delta x,y_{0}+\delta y)-u(x_{0},y_{0})}}{\delta x+i\delta y}+i\frac{{v(x_{0}+\delta x,y_{0}+\delta y)-v(x_{0},y_{0})}}{\delta x+i\delta y}$$
Take Taylor expansion of $u$ and $v$.
$$u(x_{0}+\delta x,y_{0}+\delta y)\approx u(x_{0},y_{0})+\frac{\partial u(x_{0},y_{0})}{\partial x}\delta x+\frac{\partial u(x_{0},y_{0})}{\partial y}\delta y$$
$$v(x_{0}+\delta x,y_{0}+\delta y)\approx v(x_{0},y_{0})+\frac{\partial v(x_{0},y_{0})}{\partial x}\delta x+\frac{\partial v(x_{0},y_{0})}{\partial y}\delta y$$
$$f'(z_{0})=\frac{{\delta x \frac{\partial u}{\partial x}-\delta y \frac{\partial u}{\partial y}}}{\delta x+i\delta y}+i \frac{{\delta x \frac{\partial v}{\partial x}+\delta y \frac{\partial v}{\partial y}}}{\delta x+i\delta y}.$$
$$=\frac{{\delta x\left( \frac{\partial u}{\partial x}+i \frac{\partial v}{\partial x} \right)+\delta y\left( \frac{\partial u}{\partial y}+i \frac{\partial v}{\partial y} \right)}}{\delta x+i\delta y}=\frac{{\delta x\left( \frac{\partial u}{\partial x}+i \frac{\partial v}{\partial x} \right)+i\delta y\left( -i\frac{\partial u}{\partial y}+\frac{\partial v}{\partial y} \right)}}{\delta x+i\delta y}.$$
To cancel the $\delta x$ and $\delta y$ terms, we need the conditions
$$\frac{\partial u}{\partial x}=\frac{\partial v}{\partial y}$$
$$\frac{\partial v}{\partial x}=-\frac{\partial u}{\partial y}.$$
These are the Cauchy-Riemann equations. These equations must be satisfied for a complex function to be differentiable.

The derivative $f'(z)$ can be seen as an amplification and a twist
$$f'(z)=|f'(z)|e^{i\arg(f'(z))}.$$
