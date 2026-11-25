Take $f(x,y)=x^2+y^2-xy-3x+4y$, find stationary points:
$$\frac{\partial f}{\partial x}=2x-y-3=0;\;\frac{\partial f}{\partial y}=2y-x+4$$
solve for $(x,y)$:
$$4x-2y=6$$
$$2y-x=-4$$
$$\implies 3x=2\implies x=\frac{2}{3}\implies y=-\frac{5}{3}$$
so the turning point of this function is at $\left( \frac{2}{3},-\frac{5}{3} \right)$.

Now add constraint $x+y=1$. Find minimum of $f$ subject to the new constraint.
$$g(x,y)=x+y-1=0$$
Let $L(x,y)=f(x,y)-\lambda g(x,y)$ where $\lambda$ is some unknown constant.
$$L(x,y)=x^2+y^2-xy-3x+4y-\lambda(x+y-1)$$
$$\frac{\partial L}{\partial x}=2x-y-3-\lambda=0;\; \frac{\partial L}{\partial y}=2y-x+4-\lambda=0;\; \frac{\partial L}{\partial \lambda}=-(x+y-1)=0$$
solve for $x$, $y$, $\lambda$ which gives $\lambda=1$, and minimum at $\left( \frac{5}{3},-\frac{2}{3} \right)$.
