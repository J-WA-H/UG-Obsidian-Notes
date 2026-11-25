The [metric](Tensors%20and%20Metrics.md) $g_{ab}$ embodies everything about curvature in a coordinate system, but we want a way of describing curvature that is fundamental (independent of coordinates).

Consider 2 neighbouring geodesics on flat, then curved space
![[Pasted image 20260213103300.png]]
For flat space, the distance between two points scales linearly, which it is not linear in flat space.

Consider two neighbouring geodesics $\gamma(u),\tilde{\gamma}(u)$ with separation $\zeta^a$,
![[Pasted image 20260213103820.png]]
$$\zeta^a(u)-\tilde{x}^a(u)-x^a(u)\tag{7.1} $$
The [geodesic equations](Geodesic%20Paths.md) for the two paths are
$$\gamma:\;\; \frac{d^2x^a}{du^2}+\Gamma^a_{\;bc} \frac{dx^b}{du} \frac{dx^c}{du}=0\tag{7.2} $$
$$\tilde{\gamma}:\;\; \frac{d^2\tilde{x}^a}{du^2}+\tilde{\Gamma}^a_{\;bc} \frac{d\tilde{x}^b}{du} \frac{d\tilde{x}^c}{du}=0\tag{7.3} $$
If close to the point $P$,
$$\tilde{\Gamma}^a_{\;bc}=\Gamma^a_{\;bc}+ \frac{\partial\Gamma^a_{\;bc}}{\partial x^d}\underbrace{ (\tilde{x}^d-x^d) }_{ \zeta^d }\tag{7.4} .$$
Subtracting geodesics $\tilde{\gamma}-\gamma$ gives
$$\frac{d^2\tilde{x}^a}{du^2}+\tilde{\Gamma}^a_{\;bc} \frac{d\tilde{x}^a}{du} \frac{d\tilde{x}^c}{du}-\frac{d^2x^a}{du^2}-\Gamma^a_{\;bc} \frac{dx^b}{du} \frac{dx^c}{du}=0\tag{7.5}. $$
Using $\tilde{x}^a=\zeta^a+x^a$, substituting this and approximate by keeping only first order terms in $\zeta$ gives
$$\ddot{\zeta}^a+\Gamma^a_{\;bc}\dot{x}^b\dot{\zeta}^c+\Gamma^a_{\;bc}\dot{\zeta}^b\dot{x}^c+\partial_{d}\Gamma^a_{\;bc}\zeta^d\dot{x}^b\dot{x}^c\tag{7.6}. $$
The issue is $\ddot{\zeta}^a$ is not a tensor so we need to take the [absolute derivative](Parallel%20Transport.md),
$$\frac{D^2\zeta^a}{du^2}=\frac{D}{du}\left( \frac{D\zeta^a}{du} \right)=\frac{D}{du}\left( \frac{d\zeta^a}{du} +\Gamma^a_{\;bc}\zeta^b\dot{x}^c \right)=\frac{D\dot{\zeta}^a}{du}+\frac{D}{du}(\Gamma^a_{\;bc}\zeta^b\dot{x}^c)=\frac{d^2\zeta^a}{du^2}+\Gamma^a_{\;bc}\dot{\zeta}^b\dot{x}^c+\frac{d}{du}(\Gamma^a_{\;bc}\zeta^b\dot{x}^c)+\Gamma^a_{\;ef}(\Gamma^e_{\;bc}\zeta^b\dot{x}^c)\dot{x}^f\tag{7.7}. $$
Substituting this into $(7.6)$ gives
$$\frac{D^2\zeta^a}{du^2}+(\underbrace{ \Gamma^a_{\;be}\Gamma^e_{\;cd}-\partial_{d}\Gamma^a_{\;bc}-\Gamma^a_{\;ed}\Gamma^e_{\;bc}+\partial_{b}\Gamma^a_{\;dc} }_{ R^a_{\;cbd} })\zeta^b\dot{x}^c\dot{x}^b=0\tag{7.8} $$This gives the definition of the Riemann curvature tensor
$$\frac{D^2\zeta^a}{du^2}+R^a_{\;cbd}\zeta^b\dot{x}^c\dot{x}^d=0\tag{7.9} .$$
The curvature tensor $R^a_{\;cbd}$ has a rank 4, and iff all $R^a_{\;cbd}=0$ then $\frac{D^2\zeta^a}{du^2}=0$ so the space is flat.
$$R^a_{\;cbd}=\Gamma^a_{\;bc}\Gamma^e_{\;cd}-\Gamma^a_{\;ed}\Gamma^e_{\;bc}+\partial_{b}\Gamma^a_{\;dc}-\partial_{d}\Gamma^a_{\;bc}\tag{7.10}. $$
For $R^a_{\;cbd}=0$, 
$$\frac{D^2\zeta^a}{du^2}=0\implies \frac{D\zeta^a}{du}=A\implies \zeta^a=Au+B\tag{7.11} $$which proves neighbouring geodesics separate linearly.

Consider the symmetry properties.
![[Pasted image 20260214114250.png]]
The tangent at point $P$ is a local geodesic. This is flat so $\Gamma^a_{\;bc}=0$. Its derivative doesn't vanish as the global surface around $P$ is curved.

This simplifies the curvature tensor to
$$R^a_{\;bcd}=\partial_{c}\Gamma^a_{\;db}-\partial_{d}\Gamma^a_{\;cb}\tag{7.12} $$
The fully covariant curvature tensor is
$$R_{abcd}=g_{ae}R^e_{\;bcd}=g_{ae}(\partial_{c}\Gamma^e_{\;bd}-\partial_{d}\Gamma^e_{\;cb})=\partial_{c}\Gamma_{edb}-\partial_{d}\Gamma_{ecb}\tag{7.13} .$$
Using
$$2\Gamma_{abc}=\partial_{b}g_{ac}+\partial_{c}g_{ba}-\partial_{a}g_{bc}\tag{7.14},$$
$$2R_{abcd}=\partial_{c}[\partial_{d}g_{eb}+\partial_{b}g_{de}-\partial_{e}g_{db}]-\partial_{d}[\partial_{c}g_{eb}+\partial_{b}g_{ce}-\partial_{e}g_{cb}]\tag{7.15} $$
Using symmetry properties $\partial_{c}\partial_{d}=\partial_{d}\partial_{c}$ and $g_{eb}=g_{be}$, we get
$$R_{abcd}=\frac{1}{2}[\partial_{c}\partial_{b}g_{da}-\partial_{c}\partial_{a}g_{db}-\partial_{d}\partial_{b}g_{ca}+\partial_{d}\partial_{a}g_{cb}]\tag{7.16}. $$From this we can see that
$$\begin{matrix}
R_{bacd}=-R_{abcd} \\
R_{abdc}=-R_{abcd} \\
R_{cdab}=R_{abcd}
\end{matrix}\tag{7.17}. $$
These symmetries suggest many indices are zero, for example repeated indices are zero, $R_{aacd}=-R_{aacd}\implies R_{aacd}=0$. Also $R_{abcc}=0$.

To obtain the cyclic identity,
$$\begin{matrix}
R^a_{\;bcd}=\partial_{c}\Gamma^a_{\;db}-\partial_{d}\Gamma^a_{\;cb} \\
+ \\
R^a_{\;cdb}=\partial_{d}\Gamma^a_{\;bc}-\partial_{b}\Gamma^a_{\;dc} \\
+ \\
R^a_{\;dbc}=\partial_{b}\Gamma^a_{\;cd}-\partial_{c}\Gamma^a_{\;bd}
\end{matrix}\tag{7.18} $$
This gives
$$R^a_{\;bcd}+R^a_{\;cdb}+R^a_{\;dbc}=0\tag{7.19} .$$
As these are tensor equations, they hold for all frames.

Instead of $N^4$ components in $N$-dimensions, the symmetries mean we only have
$$\frac{N^2(N^2-1)}{12}\tag{7.20} $$independent components.

For a 2D surface, $N=2$ then $R^A_{\;BCD}$ has $\frac{4\cdot {3}}{12}=1$ independent component.

We know $R_{11CD}=0=R_{AB{1}1}=R_{22CD}=R_{AB 22}$. The only components that are left are $R_{1212}=R_{2121}=-R_{2112}=-R_{1221}$. Thus we only need to calculate $R_{1212}$.
Consider a cone
$$ds^2=dr^2+r^2\sin^2 \theta_{0}d\phi \tag{7.21} $$
![[Pasted image 20260214121734.png]]
The only non-zero Christoffel symbols are, with $\omega^2=\sin^2\theta_{0}$
$$\begin{matrix}
\Gamma^r_{\;\phi \phi}=\Gamma^1_{\;22}=-r\omega^2 \\
\Gamma^\phi_{\;r\phi}=\Gamma^\phi_{\;\phi r}=\Gamma^2_{\;12}=\Gamma^2_{\;21}=\frac{1}{r}
\end{matrix}.\tag{7.22}. $$
$$R_{ABCD}=g_{AE}R^E_{\;BCD}=g_{AE}(\partial_{C}\Gamma^E_{\;BD}-\partial_{D}\Gamma^E_{\;BC}+\Gamma^F_{\;BD}\Gamma^E_{\;FC}-\Gamma^F_{\;BC}\Gamma^E_{\;FD})\tag{7.23} .$$
With the metric $g_{AB}=\mathrm{diag}(1,r^2\omega^2)$, any non-diagonal component is zero so for $R_{1212}$, $A=1$,
$$R_{12121}=g_{11}(\partial_{1}\Gamma^1_{\;22}-\partial_{2}\Gamma^1_{\;21}+\Gamma^F_{\;22}\Gamma^1_{\;F 1}-\Gamma^F_{\;21}\Gamma^1_{\;F 2})=\partial_{r}(-r\omega^2)-\frac{1}{r}(-r\omega^2)=-\omega^2+\omega^2=0\tag{7.24}. $$Even though a cone may appear to be a curved surface, it can be formed from a flat surface which is why the curvature tensor is zero.