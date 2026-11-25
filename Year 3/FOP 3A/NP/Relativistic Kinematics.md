In non-relativistic kinematics, the rest mass of a particle is given by $E=mc^2$. For a dynamic system:
$$E=mc^2+\frac{p^2}{2m}.$$
In this regime where $v\ll c$, we can define the Galilean transformation
![[Pasted image 20241116101131.png]]
$$\begin{bmatrix}
ct \\
x
\end{bmatrix}=\begin{bmatrix}
1 & 0 \\
\frac{v}{c} & 1
\end{bmatrix}\begin{bmatrix}
ct' \\
x'
\end{bmatrix}.$$

Special relativity states that $v\leq c$.

In the relativistic regime, a [[Lorentz Transforms]] is used.
![[Pasted image 20241116101325.png]]
$$\begin{bmatrix}
ct \\
x
\end{bmatrix}=\gamma\begin{bmatrix}
1 & \beta \\
\beta & 1
\end{bmatrix}\begin{bmatrix}
ct' \\
x'
\end{bmatrix}.$$
For a static object in $t'$, $x'=0$, $\Delta t=\gamma \Delta t'$.

We postulate that $\left( \frac{E}{c},\underline{p} \right)$ is a [4-vector](4-Vectors.md) 
As we defined $S'$ to be the frame where the particle is static, $E'=mc^2$ and $\underline{p}'=\underline{0}$, we get
$$\begin{bmatrix}
\frac{E}{c} \\
\underline{p}
\end{bmatrix}=\gamma\begin{bmatrix}
1 & \beta \\
\beta & 1
\end{bmatrix}\begin{bmatrix}
\frac{mc^2}{c} \\
0
\end{bmatrix}=\begin{bmatrix}
\gamma mc \\
\gamma mv
\end{bmatrix}=\gamma m\begin{bmatrix}
c \\
v
\end{bmatrix}.$$
We can use relativistic energy, $E=\gamma mc^2$ to find the non-relativistic energy.
$$E=mc^2 \frac{1}{\sqrt{ 1-\beta^2 }}$$
Using the Taylor expansion as $\beta$ us small
$$\frac{1}{\sqrt{ 1+x}}=1-\frac{1}{2}x+\mathcal{O}(x^2)\implies \frac{{1}}{\sqrt{ 1-\beta^2 }}=1+\frac{1}{2}\beta^2+\mathcal{O}(\beta^4).$$
$$\therefore E\approx mc^2\left( 1+\frac{1}{2}\beta^2 \right)=mc^2+\frac{1}{2}mv^2.$$
Now to find relativistic energy, where $p=\gamma mv=\gamma \beta mc$.
$$E^2=\frac{1}{1-\beta^2}(1-\beta^2+\beta^2)m^2c^4=m^2c^4+c^2(mc\gamma \beta)^2=m^2c^4+p^2c^2$$
$$E^2=m^2c^4+p^2c^2.$$
