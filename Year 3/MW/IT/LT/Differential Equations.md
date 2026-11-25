Differential equations can be solved using the [[Properties of Laplace Transform]], in particular the [derivatives](Derivatives%20and%20Integrals.md)
$$\mathcal{L}[f'(t)](s)=s\hat{f}(s)-f(0)$$
$$\mathcal{L}[f''(t)](s)=s^2\hat{f}(s)-sf(0)-f'(0).$$
Example: consider a particle described by $x(t)$ that is given an impulse at $t=t_{0}$, given by
$$m\ddot{x}=P\delta(t-t_{0})$$
with initial conditions $\dot{x}(0)=x(0)=0$.
Take LT of the ODE:
$$m\mathcal{L}[\ddot{x}(t)](s)=P\mathcal{L}[\delta(t-t_{0})](s)$$
$$m[s^2\hat{x}(s)-sx(0)-x'(0)]=Pe^{-st_{0}}$$
Applying boundary conditions
$$ms^2\hat{x}(s)=Pe^{-st_{0}}\implies \hat{x}(s)=\frac{P}{m} \frac{e^{-st_{0}}}{s^2}$$
Taking the inverse LT, looking at [[Common Laplace Transforms]] and the shifting property gives
$$x(t)=\frac{P}{m}(t-t_{0})\Theta(t-t_{0}).$$
Example 2:
$$y''(t)+3y'(t)+2y(t)=2-2\Theta(t-t_{0})$$
with boundary conditions $y(0)=0$, $y'(0)=2$.
$$\mathcal{L}[y''(t)](s)+3\mathcal{L}[y'(t)](s)+2\mathcal{L}[y(t)](s)=\mathcal{L}[2](s)-2\mathcal{L}[\Theta(t-t_{0})](s)$$
$$[s^2\hat{y}(s)-sy(0)-y'(0)]+3[s\hat{f}(s)-f(0)]+2\hat{y}(s)=\frac{2}{s}-\frac{2e^{-s}}{s}.$$
Applying boundary conditions:
$$[s^2\hat{y}(s)-2]+3s\hat{y}(s)+2\hat{y}(s)=\frac{{2-2e^{-s}}}{s}$$
$$\hat{y}(s)[s^2+3s+2]-2=\frac{{2-2e^{-s}}}{s}\implies \hat{y}(s)=\frac{{2-2e^{-s}+2s}}{s(s^2+3s+2)}$$
$$=\frac{{2-2e^{-s}+2s}}{s(s+2)(s+1)}=\frac{{2(s+1)-2e^{-s}}}{s(s+2)(s+1)}=\frac{2}{s(s+2)}-\frac{2e^{-s}}{s(s+1)(s+2)}.$$
Using partial fractions,
$$\hat{y}(s)=\frac{1}{s}-\frac{1}{s+2}-\frac{e^{-s}}{s}+\frac{2e^{-s}}{s+1}-\frac{e^{-s}}{s+2}$$
$$\implies y(t)=1-e^{-2t}-\Theta(t-1)+2e^{-(t-1)}\Theta(t-1)-e^{-2(t-1)}\Theta(t-1)$$
$$=1-e^{-2t}-\Theta(t-1)[2e^{-(t-1)}-e^{-2(t-1)}-1].$$
This uses the property $\mathcal{L}[f(t-t_{0})\Theta(t-t_{0})](s)=e^{-st_{0}}\hat{f}(s)$.

Example 3:
Consider the system of ODEs:
$$L\ddot{q}_{1}(t)+M\ddot{q}_{2}(t)+\frac{1}{C}q_{1}(t)=0$$
$$M\ddot{q}_{1}(t)+L\ddot{q}_{2}(t)+\frac{1}{C}q_{2}(t)=0$$
with boundary conditions $q_{1}(0)=\dot{q}_{1}(0)=0$, $q_{2}(0)=V_{0}C$, $\dot{q}_{2}(0)=0$. 
Taking LT of both equations gives
$$L[s^2\hat{q}_{1}(s)-sq_{1}(0)-\dot{q}_{1}(0)]+M[s^2\hat{q}_{2}(s)-sq_{2}(0)-\dot{q}_{2}(0)]+\frac{1}{C}\hat{q}_{1}(s)=0$$
$$M[s^2\hat{q}_{1}(s)-sq_{1}(0)-\dot{q}_{1}(0)]+L[s^2\hat{q}_{2}(s)-sq_{2}(0)-\dot{q}_{2}(0)]+\frac{1}{C}\hat{q}_{2}(s)=0$$
Applying boundary conditions gives
$$Ls^2\hat{q}_{1}(s)+M[s^2\hat{q}_{2}(s)-sV_{0}C]+\frac{1}{C}\hat{q}_{1}(s)=0$$
$$\implies\left( Ls^2+\frac{1}{C} \right)\hat{q}_{1}(s)+Ms^2\hat{q}_{2}(s)=MV_{0}Cs$$
for the second equation
$$Ms^2\hat{q}_{1}(s)+\left( Ls^2+\frac{1}{C} \right)\hat{q}_{2}(s)=LV_{0}Cs.$$
This gives a set of linear simultaneous equations, so this can be written in matrix notation
$$\begin{bmatrix}
Ls^2+\frac{1}{C} & Ms^2 \\
Ms^2 & Ls^2+\frac{1}{C}
\end{bmatrix}\begin{bmatrix}
\hat{q}_{1}(s) \\
\hat{q}_{2}(s)
\end{bmatrix}=V_{0}Cs\begin{bmatrix}
M \\
L
\end{bmatrix}.$$
Rearranging this gives
$$\begin{bmatrix}
\hat{q}_{1}(s) \\
\hat{q}_{2}(s)
\end{bmatrix}=\frac{1}{\left( Ls^2+\frac{1}{C} \right)^2-M^2s^4}\begin{bmatrix}
Ls^2+\frac{1}{C} & -Ms^2 \\
-Ms^2 & Ls^2+\frac{1}{C}
\end{bmatrix}.$$
$$\therefore \hat{q}_{1}(s)=\frac{MV_{0}s}{\left( Ls^2+\frac{1}{C}-Ms^2 \right)\left( Ls^2+\frac{1}{C}+Ms^2 \right)}$$
$$\hat{q}_{2}(s)= \frac{sV_{0}C}{\left[ s^2(L-M)+\frac{1}{C} \right][(L+M)s^2+\frac{1}{C}]}.$$
$$\therefore q_{1}=\frac{V_{0}C}{2}\left[ \cos\left( \frac{t}{\sqrt{ C(L+M) }} \right)-\cos\left( \frac{t}{\sqrt{ C(L-M) }} \right) \right].$$
Example 4: Bessel Functions
The Bessel equation of order $\alpha$ is
$$x^2\ddot{y}(x)+x\dot{y}(x)+(x^2+\alpha^2)y(x)=0.$$
Take order zero equation and solve:
$$t\ddot{y}(t)+\dot{y}(t)+ty(t)=0$$
with boundary conditions $y(0)=1$, $\dot{y}(0)=0$.
Using the property 
$$\mathcal{L}[tf(t)](s)=(-1) \frac{d\hat{f}}{ds},$$
$$\mathcal{L}[t\ddot{y}(t)](s)=- \frac{d}{ds}[s^2\hat{y}(s)-sy(0)-\dot{y}(0)]=-2s\hat{y}(s)-s^2 \frac{d\hat{y}}{ds}+y(0)$$
$$\mathcal{L}[ty(t)](s)=-\frac{d\hat{y}}{ds}.$$
Sub into equation:
$$-2s\hat{y}(s)-s^2 \frac{d\hat{y}}{ds}+y(0)+s\hat{y}(s)-y(0)-\frac{d\hat{y}}{ds}=0$$
$$-(s^2+1) \frac{d\hat{y}}{ds}-s\hat{y}(s)=0$$
$$\int\frac{d\hat{y}}{\hat{y}}=-\int \frac{sds}{s^2+1}$$
$$\ln \hat{y}=C-\frac{1}{2}\ln(s^2+1)\implies \hat{y}(s)=\frac{C}{\sqrt{ s^2+1 }}.$$
Rewrite $\hat{y}(s)$,
$$\hat{y}(s)=\frac{C}{s} \frac{1}{\sqrt{ 1+\frac{1}{s^2} }}.$$
Expand as a Taylor series around $\frac{1}{s^2}=0$,
$$\hat{y}(s)\approx \frac{C}{s}\left( 1-\frac{1}{2s^2}+\frac{3}{8s^4}+\mathcal{O}\left( \frac{1}{s^6} \right) \right)=\sum_{n=0}^{\infty}(-1)^{n} \frac{(2n)!}{(n!)^22^{2n}} \frac{1}{s^{2n+1}}.$$
Recall
$$\mathcal{L}\left[ \sum_{n=0}^{\infty} \frac{\alpha_{n}}{n!}t^{n} \right](s)=\sum_{n=0}^{\infty} \frac{\alpha_{n}}{s^{n+1}}$$
Shift $n\to 2k$.
$$\mathcal{L}\left[ \sum_{k=0}^{\infty} \frac{\alpha_{2k}t^{2k}}{(2k)!} \right](s)=\sum_{k=0}^{\infty} \frac{\alpha_{2k}}{s^{2k+1}}\therefore \alpha_{n}=\frac{(-1)^{k}(2k)!}{(k!)^22^{2k}}$$$$\therefore y(t)=C\sum_{k=0}^{\infty} \frac{(-1)^{k}}{(k!^2)} \left( \frac{t}{2} \right)^{2k}.$$
This is the Bessel function of the first kind - $y(t)=CJ_{0}(t)$.

