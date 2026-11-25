Consider a beam splitter with mode $\hat{a}_{1}$ associated with $e^{ ikx }$ and mode $\hat{a}_{0}$ associated with $e^{ -iky }$,
![[Pasted image 20251107180233.png]]
Non-linear coupling in the restricted region where the beams overlap is modelled by the Hamiltonian $\hat{H}=\hat{H}_{0}+\hat{H}_{1}+\hat{H}_{c}$.
$$\hat{H}_{0}=\hbar \omega \hat{a}^{\dagger}_{0}\hat{a}_{0},\;\hat{H}_{1}=\hbar \omega \hat{a}^{\dagger}_{1}\hat{a}_{1},\;\hat{H}_{c}=\hbar \omega_{c}(e^{ i\phi }\hat{a}^{\dagger}_{0}\hat{a}_{1}+e^{ -i\phi }\hat{a}_{1}^{\dagger}\hat{a}_{0}).\tag{13.1} $$
This reduces to $\hat{H}_{c}$ in the [interaction picture](Atom-Field%20Interactions.md) defined by
$$\hat{U}_{I}=e^{ i(\hat{H}_{0}+\hat{H}_{1})t/\hbar }.\tag{13.2} $$
For a time independent $\hat{H}$, a general operator $\hat{O}$ with no explicit time dependence evolves from the Heisenberg picture
$$\hat{O}(t)=e^{ i\hat{H}t/h }\hat{O}(0)e^{ -i\hat{H}t/\hbar }.\tag{13.3} $$
The time derivative is given by
$$\frac{d\hat{O}(t)}{dt}=\frac{i}{\hbar}[\hat{H}e^{ i\hat{H}t/\hbar }\hat{O}(0)e^{ -i\hat{H}t/\hbar }-e^{ i\hat{H}t/\hbar }\hat{O}(0)e^{ -i\hat{H}t/\hbar }\hat{H}]=\frac{i}{\hbar}[\hat{H}\hat{O}(t)-\hat{O}(t)\hat{H}]=\frac{i}{\hbar}[\hat{H},\hat{O}(t)] \tag{13.4} .$$
This reduces to the Heisenberg equation of motion.

Recursively, this implies
$$\frac{d^2\hat{O}}{dt^2}=\left( \frac{i}{\hbar} \right)^2[\hat{H},[\hat{H},\hat{O}(t)]],\; \frac{d^3\hat{O}}{dt^3}=\left( \frac{i}{\hbar} \right)^3[\hat{H},[\hat{H},[\hat{H},\hat{O}]]].\tag{13.5} $$
These derivatives can be evaluated at $t=0$ to give a Taylor series
$$\hat{O}(t)=\sum_{n=0}^{\infty} \frac{t^{n}}{n!} \left. \frac{d^n\hat{O}(t)}{dt^n} \right|_{t=0}.\tag{13.6} $$
Campbell-Baker-Hausdorff lemma: Simplifying $\hat{O}(0)$ to $\hat{O}$, the Taylor series can be expressed as
$$e^{ i\hat{H}t/\hbar }\hat{O}e^{ -i\hat{H}t/\hbar }=\hat{O}+\frac{it}{\hbar}[\hat{H},\hat{O}]+\frac{1}{2}\left( \frac{it}{\hbar} \right)^2[\hat{H},[\hat{H},\hat{O}]]+\frac{1}{3!}\left( \frac{it}{\hbar} \right)^3[\hat{H},[\hat{H},{[\hat{H},\hat{O}]}]]+\dots\tag{13.7} $$
For example with annihilation operators,
$$\begin{matrix}
[\hat{H}_{c},\hat{a}_{0}]=-e^{ -i\phi }\hbar \omega_{c}\hat{a}_{1}, & [\hat{H}_{c},\hat{a}_{1}]=-e^{ -i\phi }\hbar \omega_{c}\hat{a}_{0} \\
[\hat{H}_{c},[\hat{H}_{c},\hat{a}_{0}]]=(\hbar \omega_{c})^2\hat{a}_{0}, & [\hat{H}_{c},[\hat{H}_{c},\hat{a}_{1}]]=(\hbar \omega_{c})^2\hat{a}_{1}
\end{matrix}.\tag{13.8} $$
Using the commutators with the Campbell-Baker-Hausdorff lemma,
$$\begin{matrix}
\hat{a}_{0}(t)=\cos(\omega_{c}t)\hat{a}_{0}(0)-ie^{ i\phi }\sin(\omega_{c}t)\hat{a}_{1}(0) \\
\hat{a}_{1}(t)=-ie^{ -i\phi }\sin(\omega_{c}t)\hat{a}_{0}(0)+\cos(\omega_{c}t)\hat{a}_{1}(0)
\end{matrix}.\tag{13.9} $$
Consider $\omega_{c}t_{I}=\frac{\pi}{4}$, $\phi=\pi$,
$$\begin{matrix}
\hat{a}_{0}(t_{I})=\frac{1}{\sqrt{ 2 }}[\hat{a}_{0}(0)+i\hat{a}_{1}(0)] \\
\hat{a}_{1}(t_{I})=\frac{1}{\sqrt{ 2 }}[i\hat{a}_{0}(0)+\hat{a}_{1}(0)]
\end{matrix}\tag{13.10} .$$
We can think of the total interaction time $t_{F}$ as the path length over the speed of light in the medium. We typically think in terms of a unitary operator connecting input to output,
$$\hat{U}=e^{ i\pi/4 }(\hat{a}_{0}^{\dagger}\hat{a}_{1}+\hat{a}_{1}^{\dagger}\hat{a}_{0})\tag{13.11} .$$
This has phase shifts appropriate for a beam splitter made of a single dielectric layer. 

Using the conventions $\hat{a}_{0}=\hat{a}_{0}(0)$, $\hat{a}_{1}=\hat{a}_{1}(0)$, $\hat{a}_{2}=\hat{a}_{0}(t_{I})$, $\hat{a}_{3}=\hat{a}_{1}(t_{I})$. The relations $(13.10)$ can be inverted,
$$\begin{matrix}
\hat{a}_{0}=\frac{1}{\sqrt{ 2 }}(\hat{a}_{2}-i\hat{a}_{3}) \\
\hat{a}_{0}^{\dagger}=\frac{1}{\sqrt{ 2 }}(\hat{a}_{2}^{\dagger}+i\hat{a}_{3}^{\dagger})
\end{matrix}\tag{13.12}. $$
Consider zero photons in $\hat{a}_{0}$ and one photon in $\hat{a}_{1}$,
$$\ket{0}_{0}\ket{1} _{1}=\hat{a}^{\dagger}_{1}\ket{0}_{0}\ket{0}_{1}.\tag{13.13} $$
The effect of the beam splitter equivalent to acting with $\hat{a}_{1}^{\dagger}$ on $\ket{0}_{2}\ket{0}_{3}=\ket{0}_{0}\ket{0}_{1}$.

The input state therefore transforms to the output state as
$$\ket{0}_{0}\ket{1}_{1}\to \frac{1}{\sqrt{ 2 }}(i\ket{1} _{2}\ket{0} _{3}+\ket{0} _{2}\ket{1} _{3}).\tag{13.14} $$
The absence of coincidence counts give evidence for single-photon input states. The output state is an entangled state.

The $\ket{0}_{0}\ket{1}_{1}$ input state can be expressed as a product of the states of the 0,1 subsystems - a product state.

The $(i\ket{1}_{2}\ket{0}_{3}+\ket{0}_{2}\ket{1}_{3})/\sqrt{ 2 }$ output state cannot be expressed as a product of the 2,3 subsystems - an entangled state.

Such factorisability extends to the density operator formulation. If the density operator can be expressed as a tensor product of density operators of the subsystems it is a product state
$$\rho=\rho_{0}\rho_{1}=\rho_{0}\otimes \rho_{1}.\tag{13.15} $$
The reduced density operator is obtained by tracing over the mode 3 degrees of freedom of the output state (partial trace),
$$\rho_{R}=\sum_{n=0}^{\infty} \;_{3}\bra{n} \rho \ket{n} _{3}.\tag{13.16} $$
Here $\rho$ for the output state is given by
$$\rho=\frac{1}{2}(\ket{1} _{22}\bra{1}\otimes \ket{0}_{33}\bra{0}+i\ket{1}_{22}\bra{0}\otimes \ket{0}_{33}\bra{1} -i\ket{0} _{22}\bra{1} \otimes \ket{1} _{33}\bra{0} +\ket{0} _{22}\bra{0} \otimes \ket{1} _{33}\bra{1}  ).\tag{13.17} $$
$$\rho_{R}=\sum_{n=0}^{\infty}\;_{3}\bra{n} \rho \ket{n} _{3}=\frac{1}{2}(\ket{1} _{22}\bra{1} +\ket{0} _{22}\bra{0}  ).\tag{13.18} $$
The result is a completely mixed state. This is a signature of entanglement with other systems.

Consider $\ket{1}_{0}\ket{1}_{1}=\hat{a}_{0}^{\dagger}\hat{a}_{1}^{\dagger}\ket{0}_{0}\ket{0}_{1}$. The effect of the beam splitter is equivalent to acting
$$\hat{a}_{0}^{\dagger}\hat{a}_{1}^{\dagger}=\frac{(\hat{a}_{2}^{\dagger}+i\hat{a}_{3}^{\dagger})(i\hat{a}_{2}^{\dagger}+\hat{a}_{3}^{\dagger})}{2}=\frac{i(\hat{a}_{2}^{\dagger}\hat{a}_{2}^{\dagger}+\hat{a}_{3}^{\dagger}\hat{a}_{3}^{\dagger})}{2}\tag{13.19} $$on $\ket{0}_{2}\ket{0}_{3}$.
$$\ket{1}_{0}\ket{1}_{1} \to \frac{i}{\sqrt{ 2 }}(\ket{2}_{2}\ket{0}_{3} +\ket{0} _{2}\ket{2} _{3}  ).\tag{13.20}$$
Consider 
$$\ket{0} _{0}\ket{n} _{1}=\left[ \frac{(\hat{a}_{1}^{\dagger})^n}{n!} \right]\ket{0} _{0}\ket{0} _{1}.\tag{13.21} $$As $\hat{a}_{1}^{\dagger}=\frac{i\hat{a}_{2}^{\dagger}+\hat{a}_{3}^{\dagger}}{\sqrt{ 2 }}$ we can carry out a binomial expansion,
$$(\hat{a}_{1}^{\dagger})^{n}=\sum_{j=0}^{n} \frac{i^{j}}{2^{n/2}} \frac{n!}{j!(n-j)!}(\hat{a}_{2}^{\dagger})^{j}(\hat{a}^{\dagger}_{3})^{n-j}.\tag{13.22} $$
The resulting state is
$$\ket{0} _{0}\ket{n} _{1}\to \sum_{j=0}^{n} \frac{i^{j}}{2^{n/2}} \sqrt{ \frac{n!}{j!(n-j)!} }\ket{j} _{2}\ket{n-j} _{3}.\tag{13.23} $$Populations correspond to a binomial distribution between the output ports for the total photon number $n$.

Similarly,
$$\ket{0} _{0}\ket{\alpha}_{1}=e^{ \alpha \hat{a}_{1}^{\dagger}-\alpha ^{*}\hat{a}_{1} }\ket{0} _{0}\ket{0} _{1}.\tag{13.24} $$
Recast the displacement operator as
$$e^{ \alpha(i\hat{a}_{2}^{\dagger}+\hat{a}_{3}^{\dagger})-\alpha ^{*}(-i\hat{a}_{2}+\hat{a}_{3})/\sqrt{ 2 } }=e^{ (i\alpha \hat{a}_{2}^{\dagger}+i\alpha ^{*}\hat{a}_{2})/\sqrt{ 2 } }e^{ (\alpha \hat{a}_{3}^{\dagger}-\alpha ^{*}\hat{a}_{3}) /\sqrt{ 2 }}.\tag{13.25} $$
This can be used to determine
$$e^{ (i\alpha \hat{a}_{2}^{\dagger}+i\alpha ^{*}\hat{a}_{2}) /\sqrt{ 2 }}\ket{0} _{2}e^{ (\alpha \hat{a}_{3}^{\dagger}-\alpha ^{*}\hat{a}_{3})/\sqrt{ 2 } }.\tag{13.26} $$
The resulting state is a product state of coherent states of half intensity $\frac{|\alpha|^2}{2}$, $\ket{0}_{0}\ket{\alpha}_{1}\to \ket{\frac{i\alpha}{\sqrt{ 2 }}}_{2}\ket{\frac{\alpha}{\sqrt{ 2 }}}_{3}$.

Classical like input state becomes product of classical-like output states.
