We have a linear chain of $N$ identical atoms of mass $m$ in equilibrium positions $a,2a,\dots,Na$. Each atom is displaced from its position by $y_{1},y_{2},\dots,y_{N}$. Impose periodic boundary conditions $y_{0}=y_{N}$, in general $y_{N+\ell}=y_{\ell}$.

The Hamiltonian of the linear chain is
$$H(y_{1},y_{2},\dots,y_{N})=\sum_{\ell=1}^{N} \frac{p_{\ell}^2}{2m}+V(y_{1},y_{2},\dots ,y_{N})\tag{16.1}. $$
Lets define a translation operator on a wavefunction $f(y_{2})$,
$$\hat{T}f(y_{\ell})=f(y_{\ell+1})\implies \hat{T}^{-1}f(y_{\ell})=f(y_{\ell-1}),\;\forall\;\ell=1,\dots,N\tag{16.2}. $$
The Hamiltonian is translationally invariant so it commutes with $\hat{T}$,
$$[H,T]=0=HT-TH\implies HTT^{-1}=THT^{-1}\implies H=THT^{-1}\tag{16.3}. $$
This gives
$$\hat{T}H(y_{1},y_{2},\dots,y_{N-1},y_{N})T^{-1}=H(y_{1},y_{2},\dots,y_{N})\tag{16.4} .$$
In general it holds that $H(y_{m},y_{m+1},\dots ,y_{N},y_{1},\dots,y_{m-1})=H(y_{1},y_{2},\dots,y_{N})$.

For the potential energy, translational invariance implies
$$V(y_{m},y_{m+1},\dots,y_{N},y_{1},\dots,y_{m-1})=V(y_{1},y_{2},\dots,y_{N})\tag{16.5} $$
We expand $V$ in a Taylor series,
$$V(y_{1},\dots,y_{N})=V(0,\dots,0)+\sum_{\ell=1}^{N}y_{\ell} \left.\frac{\partial V(y_{1},\dots,y_{N})}{\partial y_{\ell }}\right|_{y_{\ell}=0}+\frac{1}{2}\sum_{\ell,m}y_{\ell}y_{m}\left. \frac{\partial^2V(y_{1},\dots,y_{N})}{\partial y_{\ell}\partial y_{m}}\right|_{y_{j}=0}\tag{16.6}. $$
Using $\frac{\partial V}{\partial y_{\ell}}=-F_{\ell}=0$ since we are at equilibrium at $y_{\ell}=0$.

The first term is a constant, which doesn't affect the physics so set $V(0,\dots,0)=0$. 
$$\therefore V(y_{1},\dots,y_{N})\simeq \frac{1}{2} \sum_{\ell,m} \left.\frac{\partial^2V}{\partial y_{\ell}\partial y_{m}}\right|_{y_{j}=0}=\frac{1}{2}\sum_{\ell,m}y_{\ell}V_{\ell m}y_{m}\tag{16.7}. $$
The Hessian matrix $V_{\ell m}$ gives information about the frequency of vibrations. We want to find the eigenvectors of $V_{\ell m}$. 
$$V=\frac{1}{2}\sum_{m\ell}y_{m}V_{m\ell}y_{\ell}=\frac{1}{2}\sum_{\ell}m\omega_{\ell}^2y_{\ell}y_{m}\tag{16.8}. $$
$$\hat{V}\ket{u_{k}}=V_{k}\ket{u_{k}} \implies \sum_{\ell}V_{m\ell}U_{k\ell}=V_{k}U_{km}\tag{16.9}. $$
We can decompose the Hessian matrix to
$$\hat{V}=\sum_{k}\ket{u_{k}} \bra{u_{k}} \tag{16.10}=\sum_{\ell} V_{k}\begin{bmatrix}
u_{k 1} \\
u_{k 2}
\end{bmatrix}\begin{bmatrix}
u_{k 1}^{*} & u_{k 2}^{*}
\end{bmatrix}=V_{1}\begin{bmatrix}
u_{11} \\
u_{22}
\end{bmatrix}\begin{bmatrix}
u_{11}^{*} & u_{22}^{*}
\end{bmatrix}+V_{2}\begin{bmatrix}
u_{21} \\
u_{22}
\end{bmatrix}\begin{bmatrix}
u_{21}^{*} & u_{22}^{*}
\end{bmatrix}.$$
Eigenvectors need to be orthonormal and form a complete basis set. This gives
$$V=\frac{1}{2}\begin{bmatrix}
y_{1} & y_{2}
\end{bmatrix}\begin{bmatrix}
V_{11} & V_{12} \\
V_{21} & V_{22}
\end{bmatrix}\begin{bmatrix}
y_{1} \\
y_{2}
\end{bmatrix}=\frac{1}{2}\begin{bmatrix}
y_{1} & y_{2}
\end{bmatrix}\sum_{k}\begin{bmatrix}
u_{k 1} \\
u_{k 2}
\end{bmatrix}\begin{bmatrix}
u_{k 1}^{*} & u_{k 2}^{*}
\end{bmatrix}\begin{bmatrix}
y_{1} \\
y_{2}
\end{bmatrix}.\tag{16.11} $$
$$V=\frac{1}{2}\sum_{k}V_{k}\underbrace{ \begin{bmatrix}
y_{1} & y_{2}
\end{bmatrix}\begin{bmatrix}
u_{k 1} \\
u_{k 2}
\end{bmatrix} }_{ Y_{k} }\underbrace{ \begin{bmatrix}
u_{k 1}^{*} & u_{k 2}^{*}
\end{bmatrix}\begin{bmatrix}
y_{1} \\
y_{2}
\end{bmatrix} }_{ Y_{k}^{*} }\tag{16.12}. $$
$$Y_{k}=u_{k\ell}y_{\ell}+u_{k\ell}y_{\ell}=\sum_{\ell}u_{k\ell}y_{\ell}\tag{16.13}. $$
$$\implies V=\frac{1}{2}\sum_{k=1}^{N}V_{k}Y_{k}Y_{k}^{*}\tag{16.14}. $$
The kinetic energy is
$$T=\frac{1}{2m}\sum_{\ell}p_{\ell}^2=\frac{1}{2m}\begin{bmatrix}
p_{1}^{\dagger} & p_{2}^{\dagger}
\end{bmatrix}\begin{bmatrix}
p_{1} \\
p_{2}
\end{bmatrix}=\frac{1}{2m}\sum_{k}\begin{bmatrix}
p_{1} & p_{2}
\end{bmatrix}\begin{bmatrix}
u_{k 1} \\
u_{k 2}
\end{bmatrix}\begin{bmatrix}
u_{k 1}^{*} & u_{k 2}^{*}
\end{bmatrix}\begin{bmatrix}
p_{1} \\
p_{2}
\end{bmatrix}=\frac{1}{2}\sum_{k}\mathbb{P}_{k}\mathbb{P}^{\dagger}_{k}\tag{16.15}.  $$
This gives $\mathbb{P}_{k}=\sum_{\ell=1}^{N}U_{k\ell}^{\dagger}p_{\ell}$. This gives the Hamiltonian
$$H=\sum_{k}\left( \frac{1}{2m}\mathbb{P}_{k}\mathbb{P}_{k}^{\dagger}+\frac{1}{2}m\omega_{k}^2Y_{k}Y_{k}^{\dagger} \right)\tag{16.16}. $$
The new variables are $Y_{q},\mathbb{P}_{q}$, with $[Y_{q},\mathbb{P}_{k}]=i\hbar\delta_{qk}$. We can define new [creation and annihilation](Boson%202nd%20Quantisation.md),
$$A_{q}=\frac{1}{\sqrt{ 2m\hbar \omega_{q} }}(m\omega_{q}Y_{q}+i\mathbb{P}_{q}^{\dagger}),\qquad A_{q}^{\dagger}=\frac{1}{\sqrt{ 2m\hbar \omega_{q} }}(m\omega_{q}Y_{q}-i\mathbb{P}_{q})\tag{16.17}. $$
We have a linear chain in $V(y_{1},\dots,y_{N})$. For $V_{m\ell}$, the important quantity is $m-\ell$.
$$\left. \frac{\partial^2V}{\partial y_{m}\partial_{\ell}} \right|_{y_{j}=0}=\left. \frac{\partial^2V}{\partial y_{m-1}\partial_{\ell-1}} \right|_{y_{j}=0}=\dots=\left. \frac{\partial^2V}{\partial y_{m-i}\partial_{\ell-i}} \right|_{y_{j}},\;i=1,2,\dots \tag{16.18} $$
This means $V_{m,\ell}=V_{m-1,\ell-1}= \dots=V_{m-m,\ell-m}=V_{N,\ell-m}=\mathcal{V}_{\ell-m}$ where
$$V_{m,\ell}=\begin{cases}
\mathcal{V}_{l-m} & 1\leq m<\ell\leq N \\
\mathcal{V}_{N+\ell-m} & 1\leq \ell \leq m\leq N
\end{cases}\tag{16.19} .$$
Diagonalising the Hessian gives
$$V_{k\ell}=\frac{e^{ ik\ell a }}{\sqrt{ N }},\qquad Y_{q}=\sum_{\ell}U_{q\ell}y_{\ell}=\sum_{\ell} \frac{e^{ iq\ell a }}{\sqrt{ N }}y_{\ell}\tag{16.20}. $$
This implies $k$ is quantised.

We have
$$\sum_{\ell=1}^{N}V_{m\ell} \frac{e^{ ik\ell a }}{\sqrt{ N }}=\sum_{\ell=1}^{m}\mathcal{V}_{N+\ell-m} \frac{e^{ ik\ell a }}{\sqrt{ N }}+\sum_{\ell=m+1}^{N}\mathcal{V}_{\ell-m} \frac{e^{ ik\ell a }}{\sqrt{ N }}\tag{16.21}. $$
Substitute $\ell'=N+\ell-m$,
$$\sum_{\ell'}V_{\ell'}e^{ ika(\ell+m-N) }+\sum_{\ell'}V_{\ell'}e^{ ika(\ell'+a) }\tag{16.22}. $$
