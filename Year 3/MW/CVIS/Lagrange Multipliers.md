Lagrange multipliers find an extremisation of a function, $f(x,y)$, in several variables subject to constraint $\phi(x,y)$.
There are two primary methods:
1. Explicitly solve $\phi$ for $y(x)$ and then substitute into $f$
2. Lagrange multipliers

Consider a set of contours of constant $f$,
![[Pasted image 20250301125225.png]]
The intersection of $\phi$ with these constant $f$ contours must be where $f$ is not extremised. If there is a touch without crossing then $f$ must be extremised.
This implies the gradient $\phi$ must be in the same direction as
$$\underline{\nabla}f=\lambda \underline{\nabla}\phi.$$
$$\implies \frac{ \partial f }{ \partial x } -\lambda \frac{ \partial \phi }{ \partial x } =0$$
$$\frac{ \partial f }{ \partial y } -\lambda\frac{\partial \phi}{\partial y}=0$$
where $\phi(x,y)=0$.
These are the [Euler-Lagrange](Functionals.md) equations for $f-\lambda \phi$.

Example: Maximise $f(x,y)=x+3y$ subject to $C(x,y)=x^2+y^2-1$.
Method 1: Direct substitution
$$C(x,y)=0\implies x^2+y^2-1=0\implies y(x)=\pm \sqrt{ 1-x^2 }$$
$$\implies f=x\pm 3\sqrt{ 1-x^2 }$$
$$\therefore \frac{df}{dx}=1\mp \frac{3x}{\sqrt{ 1-x^2 }}=0\implies{9}x^2=1-x^2\implies x=\pm \frac{1}{\sqrt{ 10 }},\;y=\pm \frac{3}{\sqrt{ 10 }}.$$
Plotting these can be used to find which one is the maximum.
![[Pasted image 20250301133015.png]]
From examining it can be seen that $\left( \frac{1}{\sqrt{ 10 }}, \frac{3}{\sqrt{ 10 }} \right)$ is the maximum.
Method 3: Lagrange multipliers
Form Lagrangian,
$$\mathcal{L}=f(x,y)-\lambda \phi(x,y)=x+3y-\lambda(x^2+y^2-1)$$
where $\lambda\in \mathbb{R}$.
Form Euler-Lagrange equations
$$\frac{\partial \mathcal{L}}{\partial\lambda}=x^2+y^2-1$$
$$\frac{\partial \mathcal{L}}{\partial x}=1-2\lambda x=0\implies x=\frac{1}{2\lambda}$$
$$\frac{\partial \mathcal{L}}{\partial y}=3-2\lambda y=0\implies y=\frac{3}{2\lambda}.$$
The constraint gives
$$x^2+y^2=1=\frac{1}{4\lambda^2}+\frac{9}{4\lambda^2}\implies{4}\lambda^2=10\implies\lambda=\pm \frac{\sqrt{ 10 }}{2}.$$
This gives the same solutions of $x=\pm \frac{1}{\sqrt{ 10 }}$, $y=\pm \frac{3}{\sqrt{ 10 }}$.

Method for Lagrange multipliers:
- Find the Euler-Lagrange equation for $\mathcal{L}=f-\lambda C$
- Express variables as functions of $\lambda$
- Substitute into constraint equation, solve for $\lambda$
- Substitute $\lambda$ to find variables.

$f(x,y)=x+3y$, $C(x,y)=x^2+y^2-1$.
Consider the increment in $f$,
$$\delta f=\frac{ \partial f }{ \partial x } \delta x+\frac{ \partial f }{ \partial y } \delta y=\begin{bmatrix}
\frac{ \partial f }{ \partial x }  & \frac{ \partial f }{ \partial y } 
\end{bmatrix}\begin{bmatrix}
\delta x \\
\delta y
\end{bmatrix}=\begin{bmatrix}
1 & 3
\end{bmatrix}\begin{bmatrix}
\delta x \\
\delta y
\end{bmatrix}.$$
$$\delta C=\begin{bmatrix}
2x & 2y
\end{bmatrix}\begin{bmatrix}
\delta x \\
\delta y
\end{bmatrix}.$$
All gradients must point in the same direction, $\underline{\nabla}f=\lambda \underline{\nabla}C$, so
$$\frac{ \partial f }{ \partial x } -\lambda \frac{ \partial C }{ \partial x } =0$$
$$\frac{ \partial f }{ \partial y } -\lambda \frac{ \partial C }{ \partial y } =0$$
For $\mathcal{L}(\dot{q}_{i},q_{i},t)$ where $i\in \mathbb{N}$, and $i\leq N$
$$\delta \mathcal{L}=\begin{bmatrix}
\frac{{\partial \mathcal{L}}}{\partial \dot{q}_{i}} & \frac{{\partial \mathcal{L}}}{\partial q_{i}} & \frac{{\partial \mathcal{L}}}{\partial t}
\end{bmatrix}\begin{bmatrix}
\delta \dot{q}_{i} \\
\delta q_{i} \\
\delta t
\end{bmatrix}.$$
The vector is $2N+1$.

Example: Pendulum
![[Pasted image 20250301140052.png]]
The Lagrangian for this system is
$$\mathcal{L}=\frac{1}{2}m(\dot{x}^2+\dot{y}^2)+mgy$$
with the constraint $x^2+y^2=l$.
$$\hat{\mathcal{L}}=\mathcal{L}-\lambda C=\frac{1}{2}m(\dot{x}^2+\dot{y}^2)+mgy-\lambda(x^2+y^2-l^2).$$
$EL_x$:
$$-\frac{d}{dt}\left( \frac{{\partial \hat{\mathcal{L}}}}{\partial \dot{x}} \right)+\frac{{\partial \hat{\mathcal{L}}}}{\partial x}=-m\ddot{x}-2\lambda x=0$$
$EL_{y}$:
$$-\frac{d}{dt}\left( \frac{{\partial \hat{\mathcal{L}}}}{\partial \dot{y}} \right)+\frac{{\partial \hat{\mathcal{L}}}}{\partial y}=-m\ddot{y}+mg-2\lambda y=0$$
$EL_{\lambda}$:
$$\frac{{\partial \hat{\mathcal{L}}}}{\partial\lambda}=x^2+y^2-l=0.$$
Consider $xEL_{x}+yEL_{y}$,
$$-m\ddot{x}x+2\lambda x^2-m\ddot{y}y+mgy-2\lambda y^2=0$$
$$-m(\ddot{x}x+\ddot{y}y)-2\lambda(x^2+y^2)+mgy=0$$
$\ddot{x}x+\ddot{y}y=-(\dot{x}^2+\dot{y}^2)$ from the fact that
$$\frac{d^2C}{dt^2}=2(x\ddot{x}+y\ddot{y}+\dot{x}^2+\dot{y}^2)=0$$
$\mathcal{L}$ does not explicitly depend on time so there is a [conserved quantity](Conservation%20Laws.md), denoted by $-E$.
$$\mathcal{L}-\dot{x} \frac{{\partial \mathcal{L}}}{\partial \dot{x}}-\dot{y} \frac{{\partial \mathcal{L}}}{\partial \dot{y}}=-E.$$
$$\frac{1}{2}m(\dot{x}^2+\dot{y}^2)+mgy-m\dot{x}^2-m\dot{y}^2=E$$
$$-\frac{1}{2}m(\dot{x}^2+\dot{y}^2)=-E-mgy$$
$$m(\dot{x}^2+\dot{y}^2)=2(E+mgy).$$
Substituting this gives
$$m(\dot{x}^2+\dot{y}^2)=2\lambda l^2-mgy$$
$$2E+2mgy=2\lambda l^2-mgy$$
$$\implies E=\lambda l^2-\frac{3}{2}mgy\implies\lambda=\frac{1}{l^2}\left( E+\frac{3}{2}mgy \right).$$
Substitute into the Euler Lagrange equation,
$$m\ddot{x}=-\frac{x}{l}(3mgy+2E)$$
$$m\ddot{y}=-\frac{y}{l}(3mgy+2E)+mg$$
Let $E=-mgy_{0}$.
Move to alternate parametisation
$$x=l\sin \theta$$$$y=l\cos \theta.$$
$$ml^2(\cos^2\theta \dot{\theta}+\sin^2\theta \dot{\theta})=-2mgl\cos \theta_{0}+2mgl\cos \theta$$
$$ml \dot{\theta}^2=-2mg(\cos \theta_{0}-\cos \theta)$$
$$\implies \dot{\theta}^2=-\frac{2g}{l}(\cos \theta_{0}-\cos \theta)$$
Take time derivative,
$$2\ddot{\theta}\dot{\theta}=\frac{d}{d\theta}\left( -\frac{2g}{l}(\cos \theta_{0}-\cos \theta) \right)\dot{\theta}=-\frac{2g}{l}\sin \theta \dot{\theta}.$$
$$\ddot{\theta}=-\frac{g}{l}\sin \theta$$
which can be solved for small $\theta$.