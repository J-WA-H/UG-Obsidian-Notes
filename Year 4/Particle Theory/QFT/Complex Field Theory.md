For a complex field, the [Lagrangian](Classical%20Field%20Theory.md) has to be altered as the scalar field $\phi\in \mathbb{C}$ so it has two real degrees of freedom. The free Lagrangian for a complex scalar field theory is
$$\mathcal{L}=(\partial_{\mu}\phi ^{*})(\partial^{\mu}\phi)-m^2\phi ^{*}\phi.\tag{2.1} $$
The main difference from the real scalar field theory is that there is no factor of $\frac{1}{2}$. A factor of $\frac{1}{2}$ is added for each real degree of freedom, so for a complex field theory, the factor is $\frac{1}{2}+\frac{1}{2}=1$ as there are 2 real degrees of freedom.

As the Lagrangian contains the field $\phi$ and its complex conjugate $\phi ^{*}$, these must be treated as two separate fields, which yields 2 Euler-Lagrange equations
$$\begin{matrix}
\phi: & (\partial_{\mu}\partial^{\mu}+m^2)\phi ^{*}=0 \\
\phi ^{*}: & (\partial_{\mu}\partial^{\mu}+m^2)\phi=0.
\end{matrix}\tag{2.2} $$
Although $(2.1)$ yields two Euler-Lagrange equations, there is only 1 independent equation, with the other being its complex conjugate.

Some properties of the Lagrangian are that its real-valued, $\mathcal{L}\in \mathbb{R}$, and it is Lorentz invariant since there are no free indices.

Noether's theorem: For every global symmetry of the action of the theory, $\exists$ a conserved current $j^{\mu}(x)$ such that
$$\partial_{\mu}j^{\mu}=0. \tag{2.3} $$This current must be conserved.

Consider the field transformation $\phi(x)\to \phi'(x)$. This transformation is a global symmetry if the action is conserved in all space,
$$S[\phi]=S[\phi'].\tag{2.4} $$
Consider the infinitesimal transformation
$$\phi(x)\to \phi'(x)=\phi(x)+\theta\delta \phi(x)\tag{2.5} $$where $\theta$ is infinitesimally small. For a transformation to be a symmetry, the action must be conserved 
$$\therefore \mathcal{L}[\phi',\partial_{\mu}\phi']=\mathcal{L}[\phi,\partial_{\mu}\phi]+\theta \partial_{\mu}I^{\mu}(\theta).\tag{2.6} $$This is possible as the last term doesn't contribute to the action. As the symmetry is global $\theta$ is not dependent on $x_{\mu}$.

Noether's current has the form
$$j^{\mu}(x)=\frac{\partial \mathcal{L}}{\partial(\partial_{\mu \phi})}\delta \phi-I^{\mu}.\tag{2.7} $$By construction this follows $(2.3)$.

The conservation of current also leads to the conservation of charge, where charge is defined by
$$Q=\int d^3x\;j^{0}\tag{2.8} .$$
From Noether's theorem,
$$\frac{dQ}{dt}=\frac{d}{dt}\int d^3x\;j^{0}=\int d^3x \frac{dj^{0}}{dt}=0\tag{2.9} $$
since $\partial_{\mu}j^{\mu}=0$ so its zeroth component $\partial_{t}j^{0}=0$.

Consider another symmetry transformation,
$$\phi(x)\to e^{ i\theta }\phi(x)\tag{2.10} $$where $\theta\in \mathbb{R}$. Since $\phi ^{*}=e^{ -i\theta }\phi ^{*}$, it is trivial that $\mathcal{L}$ is invariant. This gives
$$\begin{matrix}
\phi\cong\phi+\theta i\phi \\
\phi ^{*}\cong \phi ^{*}+\theta(-i\phi ^{*})
\end{matrix}\tag{2.11} $$for $\theta\ll 1$ and $\delta \phi=i\phi$. $j^{\mu}$ is constructed as before remembering that $\phi,\phi ^{*}$ are two separate fields,
$$j^{\mu}=(\phi ^{*}(\partial^{\mu}\phi)-(\partial^{\mu}\phi ^{*})\phi)=\phi ^{*}\stackrel{\leftrightarrow}{\partial^{\mu}}\phi \tag{2.12} $$with the shorthand notation
$$a\stackrel{\leftrightarrow}{\partial^{\mu}}b=a(\partial^{\mu}b)-(\partial^{\mu}a)b.\tag{2.13} $$
