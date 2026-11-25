Recall that a real function $f$ maps real numbers onto real numbers $f:\mathbb{R}\to \mathbb{R}$.

A functional $S$ maps a set of functions onto the real numbers.$$S:C^{n}(\mathbb{R})\to \mathbb{R}$$where $C^{n}(\mathbb{R})$ is the space of at least n differentiable functions.
$$S:f(x)\to \int_{a}^{b}F[f,f',x]dx=S[f].$$
Consider distance functionals, which give the distance between two points.
![[Pasted image 20250222132129.png]]
From Pythagoras' theorem,
$$\delta s^2=\delta x^2+\delta y^2.$$
$$\therefore \frac{dx}{dt}=\frac{\delta x}{\delta t}\implies\delta x=\frac{dx}{dt}\delta t=\dot{x}\delta t$$
$$\implies\delta s^2=\delta t^2(\dot{x}^2+\dot{y}^2).$$

To evaluate the distance functional, integrate over all infinitesimal $ds$,
$$D[\gamma]=\int_{A}^{B}ds=\int_{t_{A}}^{t_{B}} \frac{ds}{dT}dt=\int_{t_{A}}^{t_{B}}\sqrt{ \dot{x}^2+\dot{y}^2 }dt.$$
These can be used to evaluate functional derivatives. Consider the case where distance is minimised.
$$\frac{dD[\gamma]}{d\gamma}=0.$$
To find this derivative, we need to find first $D[\gamma+\delta\gamma]$:
$$\gamma(t)+\delta\gamma(t)=\begin{bmatrix}
x(t)+\delta x(t) \\
y(t)+\delta y(t)
\end{bmatrix}.$$
This means shifting paths by $\delta\gamma$ gives.
$$\sqrt{ \dot{x}^2+\dot{y}^2 }\to \sqrt{ (\dot{x}+\delta \dot{x})^2+(\dot{y}+\delta \dot{y})^2 }=\sqrt{ (\dot{x}^2+\dot{y}^2)+2(\dot{x}\delta \dot{x}+\dot{y}\delta \dot{y})+\mathcal{O}(\delta \dot{x}^2,\delta \dot{y}^2) }$$
$$\approx\sqrt{ \dot{x}^2+\dot{y}^2 }\sqrt{ 1+\frac{{2(\dot{x}\delta \dot{x}+\dot{y}\delta \dot{y})}}{\dot{x}^2+\dot{y}^\text{2}} }.$$
For small $x$,
$$\therefore \sqrt{ \dot{x}^2+\dot{y}^2 }\left( 1+\frac{2(\dot{x}\delta \dot{x}+\dot{y}\delta \dot{y})}{\dot{x}^2+\dot{y}^2} +\mathcal{O}(\delta^2)\right).$$
$$\therefore D[\gamma+\delta\gamma]=\int_{t_{A}}^{t_{B}}\sqrt{ \dot{x}^2+\dot{y}^2 }\left( 1+\frac{2(\dot{x}\delta \dot{x}+\dot{y}\delta \dot{y})}{\dot{x}^2+\dot{y}^2} \right)=D[\gamma]+\delta D$$
where
$$\delta D=\int_{t_{A}}^{t_{B}} \frac{\underline{\dot{x}}\cdot\delta \underline{\dot{x}}}{|\underline{\dot{x}}|}dt.$$
Integration by parts gives
$$\delta D=\cancelto{0}{\left[ \frac{\underline{\dot{x}}\cdot\delta \underline{x}}{|\underline{\dot{x}}|} \right]_{t_{A}}^{t_{B}}}-\int_{t_{A}}^{t_{B}} \frac{d}{dt} \left( \frac{\underline{\dot{x}}}{|\underline{\dot{x}}|} \right)\cdot\delta \underline{x}dt.$$
The bracket goes to zero as $\delta x$ does not differ from the original function as they both start and end at the same points.
![[Pasted image 20250222135007.png]]
$$\therefore \delta D=\int_{t_{A}}^{t_{B}} \frac{d}{dt}\left(  \frac{\dot{\underline{x}}}{|\underline{\dot{x}}|} \right)\cdot\delta \underline{x}dt.$$
As we are minimising the distance, we want $\delta D=0$ so we want $\frac{\dot{\underline{x}}}{|\underline{\dot{x}}|}$ to remain constant in time, i.e. the direction of the path doesn't change. This shows what is intuitive that the shortest path is a straight line.

Consider the functional
$$S[f]=\int_{a}^{b}L[f,f',x]dx.$$
For a small perturbation with $\delta f(a)=\delta f(b)=0.$
$$\delta L=\frac{\partial L}{\partial f}\delta f+\frac{\partial L}{\partial f'}\delta f'$$
$$\implies\delta S=\int_{a}^{b}\left( \frac{\partial L}{\partial f}\delta f+\frac{\partial L}{\partial f'}\delta f' \right)dx=\int_{a}^{b}\left( \frac{\partial L}{\partial f}-\frac{d}{dx}\left( \frac{\partial L}{\partial f'} \right) \right)\delta fdx+\cancelto{0}{\left[ \frac{\partial L}{\partial f'} \delta f \right]_{a}^{b}}.$$
$$\therefore \frac{\delta s}{\delta f}=\frac{\partial L}{\partial f}-\frac{d}{dx}\left( \frac{\partial L}{\partial f'} \right)$$
where $\delta S=\int_{a}^{b}dx\delta f\left( \frac{\delta s}{\delta f} \right)$.
This is the functional derivative.
For the case where $\delta S=0$,
$$\frac{\partial L}{\partial f}-\frac{d}{dx}\left( \frac{\partial L}{\partial f'} \right)=0.$$
This is the extremised functional - known as the Euler-Lagrange equation.

Example: Find the Euler-Lagrange equation for
$$S[\gamma]=\int_{0}^{1}((y')^2+y^2+2xy)dx$$
with $y(0)=0$ and $y(1)=\alpha$.
$$\frac{\partial L}{\partial y}=2y+2x;\; \frac{\partial L}{\partial y'}=2y'.$$
This gives the Euler-Lagrange equation
$$2(y+x)-2y''=0\implies y''=y+x.$$
Find the stationary function $y$.
Solving the ODE gives
$$y(x)=Ce^{x}+De^{-x}-x.$$
$$y(0)=0\implies C+D=0.$$
$$y(x)=C(e^{x}-e^{-x})-x=2C\sinh(x)-x$$
$$y(1)=\alpha \implies C(e-e^{-1})-1=\alpha$$
$$\implies y(x)=(\alpha+1) \frac{\sinh(x)}{\sinh(1)}-1.$$
