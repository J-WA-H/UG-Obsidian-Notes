Consider the single particle boson state $\phi_{0}$,
$$\underbrace{ \Phi_{n}(\vec{r}_{1},\vec{r}_{2},\dots,\vec{r}_{n}) }_{ \ket{n}  }=\phi_{0}(\vec{r}_{1})\phi_{0}(\vec{r}_{2})\dots \phi_{0}(\vec{r}_{n})\tag{11.1} $$
$$\ket{m}=\Phi_{m}(\vec{r}_{1},\dots,\vec{r}_{n},\dots \vec{r}_{m})=\phi_{0}(\vec{r}_{1})\dots \phi_{0}(\vec{r}_{n})\dots \phi_{0}(\vec{r}_{m})\tag{11.2}  $$
Define the action of the annihilation operator $a_{0}$,
$$a_{0}\ket{n} =C_{n}\ket{n-1}\tag{11.3}  .$$
We want to figure the action of $a_{0}^{\dagger}$ on a ket,$$\bra{n} a_{0}^{\dagger}=C_{n}^{*}\bra{n-1}\implies \bra{n} a_{0}^{\dagger}\ket{n-1} =C_{n}^{*}\braket{ n-1 | n-1 } =C_{n}^{*}= C_{n}^{*}\braket{ n | n } \implies \bra{n} (a_{0}^{\dagger}\ket{n-1} -C_{n}^{*}\ket{n} )=0\tag{11.4} $$$$\implies a_{0}^{\dagger}\ket{n-1} =C_{n}^{*}\ket{n} \tag{11.5}$$
Now aim to find $C_{n}$. Define the number operator $\hat{N}_{0}=a_{0}^{\dagger}a_{0}$.
$$\hat{N}_{0}\ket{n} =n\ket{n} =\hat{a}_{0}^{\dagger}\hat{a}_{0}\ket{n}=a_{0}^{\dagger}C_{n}\ket{n-1} =C_{n}^{*}C_{n}\ket{n} =|C_{n}|^2\ket{n}\implies |C_{n}|^2=n\implies C_{n}=\sqrt{ n }.\tag{11.6}  $$
This gives
$$\begin{matrix}
a_{0}\ket{n} =\sqrt{ n }\ket{n-1}  \\
a_{0}^{\dagger}\ket{n-1} =\sqrt{ n }\ket{n} 
\end{matrix}\tag{11.7} $$
We can write $\ket{n}$ in terms of $a_{0}^{\dagger}$ acting on the vacuum $\ket{0}$,
$$\ket{n} =\frac{1}{\sqrt{ n! }}(a_{0}^{\dagger})^n\ket{0}\tag{11.8}  $$
We expect boson creation and annihilation operators to satisfy
$$[a_{0},a_{0}^{\dagger}]=1.\tag{11.9} $$
Proof:
$$[a_{0},a_{0}^{\dagger}]\ket{n}= (a_{0}a_{0}^{\dagger}-a_{0}^{\dagger}a_{0})\ket{n} =a_{0}a_{0}^{\dagger}\ket{n} -a_{0}^{\dagger}a_{0}\ket{n}=a_{0}\sqrt{ n+1 }\ket{n+1} -a_{0}^{\dagger}\sqrt{ n }\ket{n-1} =\sqrt{ n+1 }\sqrt{ n+1 }\ket{n} -\sqrt{ n }\sqrt{ n }\ket{n} =\ket{n}\;\square.  $$
$$a_{i}\ket{\dots,n_{i},\dots,n_{j},\dots} =\sqrt{ n_{i} }\ket{\dots,n_{i}-1,\dots,n_{j},\dots}\tag{11.10}  $$
In general, $$[a_{j},a_{i}^{\dagger}]=\delta_{ij},\;\;[a_{j},a_{i}]=0=[a_{j}^{\dagger},a_{i}^{\dagger}].\tag{11.11} $$
