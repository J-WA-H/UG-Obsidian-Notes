Consider the basis vector for a contravariant [tensor](Tensors%20and%20Metrics.md),
$$\vec{e}_{a}=\frac{{\partial \vec{r}}}{\partial x^a}\tag{3.1}. $$For covariant tensors, $\vec{A}=A_{a}\vec{e}^a$. Consider the scalar field
$$\vec{\nabla} \phi=\frac{\partial \phi}{\partial x}\vec{i}+\frac{\partial \phi}{\partial y}\vec{j}+\frac{\partial \phi}{\partial z}\vec{k}.\tag{3.2} $$
Define the basis vectors following the gradient of the scalar field $\phi$.
![[Pasted image 20260128203138.png]]
In this case the vectors follow $\vec{i},\vec{j}$ as the axes are orthonormal. Consider a case of non-orthogonal axes,
![[Pasted image 20260128203241.png]]
Here we define $\vec{e}^a=\vec{\nabla}x^a$,
$$\vec{\nabla}\phi=\frac{\partial \phi}{\partial x^i}\vec{e}^i=\frac{\partial \phi}{\partial x^\bar{j}}\left(\frac{\partial x^\bar{j}}{\partial x^i}\vec{e}^i\right)= \frac{\partial \phi}{\partial x^\bar{j}}(\vec{\nabla}x^\bar{j})\tag{3.3} $$this gives
$$\vec{e}^\bar{j}=\vec{\nabla}x^\bar{j}=\left( \frac{\partial x^\bar{j}}{\partial x^i}\vec{e}^i \right)\tag{3.4} $$which gives the [transformation of the basis vector](Curvature%20as%20Distance.md). 
$$\therefore \vec{A}=A_{a}\vec{e}^a\to A_{\bar{b}}\vec{e}^\bar{b}=\left( \frac{\partial x^a}{\partial x^\bar{b}}A_{a} \right)\left( \frac{\partial x^\bar{b}}{\partial x^c}\vec{e}^c \right)=\frac{\partial x^a}{\partial x^c}A_{a}\vec{e}^c=\delta^a_{\;c}A_{a}\vec{e}^c=A_{a}\vec{e}^a\;\square.\tag{3.5} $$
Consider $\vec{\lambda}=\lambda^a\vec{e}_{a}=\lambda_{b}\vec{e}^b$ and $\vec{\mu}=\mu^a\vec{e}_{a}=\mu_{b}\vec{e}^b$,
$$\begin{matrix}
\vec{\lambda}\cdot \vec{\mu}=(\lambda^a\vec{e}_{a})\cdot(\mu^b\vec{e}_{b})=g_{ab}\lambda^a\mu^b \\
=(\lambda_{a}\vec{e}^a)\cdot(\mu_{b}\vec{e}^b)=g^{ab}\lambda_{a}\mu_{b} \\
=(\lambda_{a}\vec{e}^a)\cdot(\vec{\mu}^b\vec{e}_{b})=g^a_{\;b}\lambda_{a}\mu^b \\
\end{matrix}\tag{3.6}. $$
Then consider
$$\vec{e}_{i}\cdot \vec{e}^j=\frac{\partial \vec{r}}{\partial x^i}\vec{\nabla}x^j=\left( \frac{\partial x^1}{\partial x^i}\vec{i}+\frac{\partial x^2}{\partial x^i}\vec{j}+\frac{\partial x^3}{\partial x^i}\vec{k} \right)\cdot\left( \frac{\partial x^j}{\partial x^1}\vec{i}+\frac{\partial x^j}{\partial x^2}\vec{j}+\frac{\partial x^j}{\partial x^3} \right)=\frac{\partial x^j}{\partial x^i}=\delta^j_{\;i}.\tag{3.7} $$
The factor of 3 is missing since $\delta^j_{\;i}=3$.
$$\vec{\lambda}\cdot \vec{\mu}=\lambda^a\mu_{b}\vec{e}_{a}\cdot \vec{e}^b=\lambda^a\mu_{a}\delta_{a}^{\;b}=\lambda^a\mu_{a}=\lambda_{a}\mu^a=g_{ab}\lambda^a\mu^b\implies\lambda_{b}=g_{ab}\lambda^a\tag{3.8}.  $$Considering this gives
$$\lambda_{a}=g_{ab}\lambda^b=g_{ab}(g^{bc}\lambda_{c})=g_{ab}g^{bc}\lambda_{c}\tag{3.9}\implies g_{ab}g^{bc}=\delta_{a}^{\;c}.$$
For a summary of tensor algebra, the position vector is $\vec{r}=x^a\vec{e}_{a}$ transforms as
$$\begin{matrix}
x^\bar{b}=x^\bar{b}(x^a) \implies dx^\bar{b}=\left( \frac{\partial x^\bar{b}}{\partial x^a} \right)dx^a \\
A^\bar{b}=\frac{\partial x^\bar{b}}{\partial x^a}A^a \\
\vec{e}^a=\vec{\nabla}x^a \\
\frac{\partial\phi}{\partial x^\bar{b}}=\frac{\partial \phi}{\partial x^a} \frac{\partial x^a}{\partial x^\bar{b}} \\
A_{\bar{b}}=\frac{\partial x^a}{\partial x^\bar{b}}A_{a}
\end{matrix}.\tag{3.10} $$
For a generalised tensor,
$$T^{\bar{a}_{1}\bar{a}_{2}\dots \bar{a}_{r}}_{\;\;\;\;\;\;\;\;\;\;\;\;\bar{b}_{1}\bar{b}_{2} \dots\bar{b}_{s}}=\left( \frac{\partial x^{\bar{a}_{1}}}{\partial x^{a_{1}}}\dots \frac{\partial x^{\bar{a}_{r}}}{\partial x^{a_{r}}} \right)\left( \frac{\partial x^{b_{1}}}{\partial x^{\bar{b}_{1}}}\dots \frac{\partial x^{b_{s}}}{\partial x^{\bar{b}_{s}}} \right)T^{a_{1}\dots a_{r}}_{\;\;\;\;\;\;\;\;b_{1}\dots b_{s}}.\tag{3.11} $$
This is a $(r,s)$ tensor of rank $r+s$.

Linear combinations:
$$T^c_{\;d}=aA^c_{\;d}+bB^c_{\;d}\tag{3.12}, A^c_{\;d},B^c_{\;d}\in(1,1)\implies T^c_{\;d}\in(1,1).$$
Proof: Transform to a new coordinate system,
$$T^{\bar{c}}_{\;\bar{d}}=aA^{\bar{c}}_{\;\bar{d}}+bB^\bar{c}_{\;\bar{d}}=a\left( \frac{\partial x^\bar{c}}{\partial x^c} \frac{\partial x^d}{\partial x^\bar{d}} \right)A^c_{\;d}+b\left( \frac{\partial x^\bar{c}}{\partial x^c} \frac{\partial x^d}{\partial x^\bar{d}} \right)B^c_{\;d}=\left( \frac{\partial x^\bar{c}}{\partial x^c} \frac{\partial x^d}{\partial x^\bar{d}}\right)(aA^c_{\;d}+bB^c_{\;d})=\left( \frac{\partial x^\bar{c}}{\partial x^c} \frac{\partial x^d}{\partial x^\bar{d}}\right)T^c_{\;d}\;\square.\tag{3.13} $$Direct (outer) product: $T^a_{\;b}=A^aB_{b}$.
$$T^\bar{a}_{\bar{b}}=\left( \frac{\partial x^\bar{a}}{\partial x^a} \right)A^a\left( \frac{\partial x^b}{\partial x^\bar{b}} \right)B_{b}=\left( \frac{\partial x^\bar{a}}{\partial x^a} \frac{\partial x^b}{\partial x^\bar{b}} \right)A^aB_{b}=\left( \frac{\partial x^\bar{a}}{\partial x^a} \frac{\partial x^b}{\partial x^\bar{b}} \right)T^a_{\;b}.\tag{3.14} $$
A general inner product (contraction): $T^{a\;cd}_{\;\;b}=A^aB_{b}C^cD^d$.
Suppose we contract over two indices
$$\begin{matrix}
T^{a\;bd}_{\;\;b}=T^{ad} & T^{a\;cb}_{\;\;b}=T^{ac} \\
T^{a\;cd}_{\;\;a}=T^{cd}
\end{matrix}.\tag{3.15} $$These are all different tensors $(3.16)$.
$$T^{\bar{a}\;\bar{c}\bar{d}}_{\;\;\bar{a}}=\frac{\partial x^\bar{a}}{\partial x^a}A^a \frac{\partial x^b}{\partial x^\bar{a}}B_{b} \frac{\partial x^\bar{c}}{\partial x^c}C^c \frac{\partial x^\bar{d}}{\partial x^d}D^d=\frac{\partial x^\bar{a}}{\partial x^a}\frac{\partial x^b}{\partial x^\bar{a}}\frac{\partial x^\bar{c}}{\partial x^c}\frac{\partial x^\bar{d}}{\partial x^d}A^aB_{b}C^cD^d=\frac{\partial x^b}{\partial x^a}\frac{\partial x^\bar{c}}{\partial x^c}\frac{\partial x^\bar{d}}{\partial x^d}T^{a\;cd}_{\;\;b}=\delta^b_{\;a}\frac{\partial x^\bar{c}}{\partial x^c}\frac{\partial x^\bar{d}}{\partial x^d}T^{a\;cd}_{\;\;b}=\frac{\partial x^\bar{c}}{\partial x^c}\frac{\partial x^\bar{d}}{\partial x^d}T^{a\;cd}_{\;\;a}. $$
This shows $T^{cd}$ is a $(2,0)$ tensor.

The inner product of 2 first order tensors is essentially a dot product,
$$\vec{A}\cdot \vec{B}=g_{ab}A^aB^b=A^aB_{a}=A_{b}B^b=g^{ab}A_{a}B_{b}=|\vec{A}||\vec{B}|\cos \chi.\tag{3.16} $$This is a scalar so must be invariant. An example is
$$ds^2=c^2d\tau^2=g_{\alpha\beta}dx^\alpha dx^\beta \tag{3.17} $$so any tensor equation keeps the fame form in any coordinate system
$$\therefore ds^2=dx^2+dy^2+dz^2=dr^2+r^2d\theta^2+r^2\sin^2\theta d\phi=g_{ij}dx^idx^j.\tag{3.18}. $$
