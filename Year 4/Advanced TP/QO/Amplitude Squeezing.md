Recall the [quadrature operators](Coherent%20States.md),
$$\hat{X}_{1}=\frac{{\hat{a}+\hat{a}^{\dagger}}}{2},\;\hat{X}_{2}=\frac{i(\hat{a}^{\dagger}-\hat{a})}{2}\tag{4.1}. $$
This is related to the number operator $\hat{N}=\hat{a}^{\dagger}\hat{a}$ by
$$\hat{X}_{1}^2+\hat{X}_{2}^2=\hat{N}+\frac{1}{2}.\tag{17.1} $$
The coherent state expectation values are
$$\langle \hat{X}_{1} \rangle =\frac{{\alpha+\alpha ^{*}}}{2},\;\langle \hat{X}_{2} \rangle =\frac{i(\alpha ^{*}-\alpha)}{2}\tag{17.2} $$
$$\langle \hat{X}_{1}^2 \rangle =\frac{{2|\alpha|^2+1+\alpha^2+\alpha ^{*2}}}{4}=\langle \hat{X}_{1} \rangle ^2+\frac{1}{4}\tag{17.3} $$
$$\langle \hat{X}_{2}^2 \rangle =\frac{{2|\alpha|^2+1-\alpha^2-\alpha ^{*2}}}{4}=\langle \hat{X}_{2} \rangle ^2+\frac{1}{4}.\tag{17.4} $$
$$\langle \hat{N} \rangle =|\alpha|^2=\langle \hat{X}_{1}^2 \rangle + \langle \hat{X}_{2}^2 \rangle -\frac{1}{2}=\langle \hat{X}_{1} \rangle ^2+\langle \hat{X}_{2} \rangle ^2.\tag{17.5}  $$
Note the presence of quantum fluctuations.
For the equivalent classical conditions, set $X_{1}=\langle \hat{X}_{1} \rangle$, $X_{2}=\langle \hat{X}_{2} \rangle$, $N=\langle \hat{N} \rangle$, $\alpha=\varrho e^{ i\phi }$ implies that, for a coherent state,
$$X_{1}=\varrho \cos \phi,\;X_{2}=\varrho \sin \phi,\;N=\varrho^2.\tag{17.6} $$
The quantities $\phi,N$ map onto a classical canonically conjugate pair as
$$\{ \phi,N \}=\frac{\partial \phi}{\partial \phi} \frac{\partial N}{\partial N}-\frac{\partial N}{\partial \phi} \frac{\partial \phi}{\partial N}=\frac{1}{2} \frac{\partial \phi}{\partial X_{1}} \frac{\partial N}{\partial X_{2}}-\frac{1}{2} \frac{\partial N}{\partial X_{1}} \frac{\partial \phi}{\partial X_{2}}=1.\tag{17.7} $$
The Poisson bracket is the classical equivalent of the commutator so it points towards the $\phi,N$ uncertainty principle. The phase is poorly defined quantally, however states with a number uncertainty less than that of a coherent state are possible.
![[Pasted image 20251121102804.png]]
The number variance in [p-representation](Quadrature%20Squeezing.md) is
$$\langle \Delta \hat{N}^2 \rangle =\langle \hat{a}^{\dagger}\hat{a} \rangle +\int d^2\alpha \;p(\alpha,\alpha ^{*})(|\alpha|^2-\langle \hat{a}^{\dagger}\hat{a} \rangle )^2\tag{17.8} $$
For a coherent state, $\langle \Delta \hat{N}^2 \rangle=\langle \hat{a}^{\dagger}\hat{a} \rangle$ and $\langle \Delta \hat{N}^2 \rangle < \langle \hat{a}^{\dagger}\hat{a} \rangle$ requires $p(\alpha,\alpha ^{*})<0$  over at least some of its domain.

The $Q$ parameter is defined by
$$Q=\frac{{\langle \Delta \hat{N}^2 \rangle -\langle \hat{N} \rangle }}{\langle \hat{N} \rangle }\tag{17.9}. $$
For $Q=0$, we have Poissonian number statistics, sub-Poissonian statistics for $Q<0$, and super-Poissonian statistics for $Q>0$.

Consider $\ket{\alpha,\xi}$, $\xi=re^{ i\theta }$, $\alpha=|\alpha|e^{ i\phi }$. If the axis (defined by $\frac{\theta}{2}$) along which the squeezing is directed is the same as that defined by $\phi$ then we can have $Q<0$.
![[Pasted image 20251121110016.png]]
It can be shown that for $\ket{\alpha,\xi}$:
- $\langle \hat{N} \rangle=|\alpha|^2+\sinh^2(r)$
- $\langle \Delta \hat{N}^2 \rangle=|\alpha \cosh(r)-\alpha ^{*}e^{ i\theta }\sinh(r)|^2+2\sinh^2(r)\cosh^2(r)$.
If $\phi=\frac{\theta}{2}$ then $\langle \Delta \hat{N}^2 \rangle=|\alpha|^2e^{ -2r }+2\sinh^2(r)\cosh^2(r)$.
If less than $\langle \hat{N} \rangle=|\alpha|^2+\sinh^2(r)$ then $Q<0$.

The amplitude squeezing condition that relates $r$ to $|\alpha|$ is
$$e^{ r }\sinh^2(r)[\cosh^2(r)+1]<2|\alpha|^2\sinh(r).\tag{17.10} $$
This can be divided through by $\sinh(r)$ if $r>0$. If the condition is fulfilled, then $Q<0$ and we hace sub-Poissonian number statisics.

