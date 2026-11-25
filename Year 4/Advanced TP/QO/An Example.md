Level Configuration:
![[Pasted image 20251205093425.png]]
The many-molecule generalisation is, within an appropriate frame, and all detuning set to zero,
$$\hat{H}=\frac{{\hbar \theta}}{2}\sum_{k=1}^{N}(\hat{\sigma}^{+}_{k}\hat{S}^{-}+\hat{S}^{+}\hat{\sigma}^{-}_{k})+\frac{{\hbar \Omega}}{2}(\hat{S}^{-}_{r}+\hat{S}^{+}_{r})\tag{22.1} $$where $\hat{\sigma}^{+}_{k}=\ket{1}_{kk}\bra{0}$, $\hat{\sigma}^{-}_{k}=\ket{0}_{kk}\bra{1}$, $\hat{S}^{+}=\ket{R}\bra{r}$, $\hat{S}^{-}=\ket{r}\bra{R}$, $\hat{S}^{+}_{r}=\ket{r}\bra{g}$, $\hat{S}^{-}_{r}=\ket{g}\bra{r}$.
This ignores molecule-molecule interactions.
We assume molecules equidistant from the Rydberg atom.

To simplify the maths, consider all energies to be in units of $\frac{\hbar \theta}{2}$,
$$\hat{H}=\sum_{k=1}^{N}(\hat{\sigma}^{+}_{k}\hat{S}^{-}+\hat{S}^{+}\hat{\sigma}^{-}_{k})+\Omega(\hat{S}^{-}+\hat{S}^{+}_{k}).\tag{22.2} $$
Here the only parameter is $\Omega$. This is the obvious mapping of generic qubits onto spin-$\frac{1}{2}$ systems. Similarly, the total angular momentum ladder operators,
$$\hat{J}^{+}_{N}=\sum_{k=1}^{N}\hat{\sigma}^{+}_{k}\tag{22.3}. $$The Hamiltonian is then
$$\hat{H}=\hat{J}^{+}_{N}\hat{S}^{-}+\hat{S}^{+}\hat{J}^{-}_{N}+\Omega(\hat{S}^{-}_{r}+\hat{S}^{+}_{r})\tag{22.4}. $$
The logical basis for two molecules is
$$\{ \ket{00} =\ket{0}_{1}\ket{0} _{2},\ket{01} ,\ket{10} ,\ket{11}  \}\tag{22.5} $$and the total angular momentum basis is $(22.6)$
$$\left\{  \ket{J_{2}=1,m_{J_{2}}=1} =\ket{11} ,\ket{J_{2}=1,m_{J_{2}}=-1} =\ket{00} , \ket{J_{2}=1,m_{J_{2}}=0}=\frac{1}{\sqrt{ 2 }}(\ket{01} +\ket{10} ),\ket{J_{2}=0,m_{J_{2}}=0} = \frac{1}{\sqrt{ 2 }}(\ket{01} -\ket{10} ) \right\}.\tag{22.6} $$
The effect of the ladder operators is as usual,
$$\hat{J}^{\pm}_{2}\ket{J_{2},m_{J_{2}}} =\sqrt{ J_{2}(J_{2}+1)-m_{J_{2}}(m_{J_{2}}\pm1) }\ket{J_{2},m_{J_{2}}\pm 1}\tag{22.7}.  $$
Ladder operators do not change the $J_{2}$ quantum number, only the $m_{J_{2}}$ quantum number, so only $m_{J}$ can change under the influence of the Hamiltonian.
![[Pasted image 20251205101104.png]]
The Hamiltonian matrix is
$$H=\begin{bmatrix}
0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & \sqrt{ 2 } & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 \\
0 & \sqrt{ 2 } & 0 & \Omega & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & \Omega & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & \sqrt{ 2 } & 0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & \sqrt{ 2 } & 0 & \Omega & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & \Omega & 0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & \Omega & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 & 0 & \Omega & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & \Omega \\
0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 & \Omega & 0
\end{bmatrix}\tag{22.8} $$
This is a block diagonal matrix, which breaks down into 2 to 3 dimensional matrices.
For the 3 dimensional case, in the basis $\{ \ket{1,0,R},\ket{1,1,r},\ket{1,1,g} \}$,
$$H=\begin{bmatrix}
0 & \sqrt{ 2 } & 0 \\
\sqrt{ 2 } & 0 & \Omega \\
0 & \Omega & 0
\end{bmatrix}\tag{22.9}. $$
$E_{0}=0,E_{\pm}=\pm \sqrt{ 2+\Omega^2 }$.
$$\vec{v}_{0}=\frac{1}{\sqrt{ 2+\Omega^2 }}\begin{bmatrix}
\Omega \\
0 \\
-\sqrt{ 2 }
\end{bmatrix},\;\vec{v}_{\pm}=\frac{1}{\sqrt{ 2(2+\Omega^2) }}\begin{bmatrix}
\sqrt{ 2 } \\
\pm \sqrt{ 2+\Omega^2 } \\
\Omega
\end{bmatrix}\tag{22.10} $$
For the 2 dimensional case,
$$H=\begin{bmatrix}
0 & \Omega \\
\Omega & 0
\end{bmatrix}\tag{22.11} $$
for $\{ \ket{1,-1,r},\ket{1,-1,g} \}$ and $\{ \ket{0,0,r},\ket{0,0,g} \}$. $E_{\pm}=\pm \Omega$,
$$u_{\pm}=\frac{1}{\sqrt{ 2 }}\begin{bmatrix}
1 \\
\pm 1
\end{bmatrix}.\tag{22.12} $$
For the logical basis and natural basis,
$$\begin{matrix}
\ket{00,g} = \ket{1,-1,g} , & \ket{10,g} = \frac{1}{\sqrt{ 2 }}(\ket{1,0,g} -\ket{0,0,g} ) \\
\ket{01,g} =\frac{1}{\sqrt{ 2 }}(\ket{1,0,g} +\ket{0,0,g} ) & \ket{11,g} =\ket{1,1,g} 
\end{matrix}\tag{22.13}. $$
The eigenbasis decomposition is
$$\begin{matrix}
\ket{0,0,g} =\frac{1}{\sqrt{ 2 }}(\ket{u^{0,0}_{+}} -\ket{u^{0,0}_{-}} ). & \ket{1,-1,g}=\frac{1}{\sqrt{ 2 }}(\ket{u^{1,-1}_{+}} -\ket{u^{1,-1}_{-}} )  \\
\ket{1,0,g} = \frac{1}{\sqrt{ 2+\Omega^2 }}\left[ \frac{\Omega}{\sqrt{ 2 }}(\ket{v^{1,0}_{+}}+\ket{v^{1,0}_{-}}  )-\sqrt{ 2 }\ket{v^{1,0}_{0}}  \right] & \ket{1,1,g} =\frac{1}{\sqrt{ 2+\Omega^2 }}\left[ \frac{\Omega}{\sqrt{ 2 }}(\ket{v^{1,1}_{+}} +\ket{v^{1,1}_{-}} )-\sqrt{ 2 }\ket{v_{0}^{1,1}}  \right]
\end{matrix}\tag{22.14} .$$
The time evolution is$$\begin{matrix}
\ket{0,0,g} =\frac{1}{\sqrt{ 2 }}(e^{ -i\Omega t }\ket{u^{0,0}_{+}} -e^{ i\Omega t }\ket{u^{0,0}_{-}} ). & \ket{1,-1,g}=\frac{1}{\sqrt{ 2 }}(e^{ -i\Omega t }\ket{u^{1,-1}_{+}} -e^{ i\Omega t }\ket{u^{1,-1}_{-}} )  \\
\ket{1,0,g} = \frac{1}{\sqrt{ 2+\Omega^2 }}\left[ \frac{\Omega}{\sqrt{ 2 }}(e^{ -i\sqrt{ 2+\Omega^2 }t }\ket{v^{1,0}_{+}}+e^{ i\sqrt{ 2+\Omega^2 }t }\ket{v^{1,0}_{-}}  )-\sqrt{ 2 }\ket{v^{1,0}_{0}}  \right] \\ \ket{1,1,g} =\frac{1}{\sqrt{ 2+\Omega^2 }}\left[ \frac{\Omega}{\sqrt{ 2 }}(e^{ -i\sqrt{ 2+\Omega^2 }t }\ket{v^{1,1}_{+}} +e^{ i\sqrt{ 2+\Omega^2 }t }\ket{v^{1,1}_{-}} )-\sqrt{ 2 }\ket{v_{0}^{1,1}}  \right]
\end{matrix}\tag{22.14} .$$
For the quantum gate conditions, we set $\Omega t=(2s+1)\pi$. This is satisfied (in redimensionalised form) when
$$t=\frac{(2s+1)\pi}{\Omega},\;\Omega=\sqrt{ \frac{2}{4n^2-1} }\theta.\tag{22.15} $$
Hence
$$\begin{matrix}
\ket{0,0,g} \to-\ket{0,0,g} , & \ket{1,-1,g} \to-\ket{1,-1,g} , & \ket{1,0,g} \to \ket{1,0,g} , & \ket{1,1,g} \to \ket{1,1,g} 
\end{matrix}.\tag{22.16} $$
Finally, we see that in the logical basis we have a controlled z-gate
$$\begin{matrix}
\ket{00,g} \to-\ket{00,g} , & \ket{01,g} \to \ket{10,g} , & \ket{10,g} \to \ket{01,g} , & \ket{11,g} \to \ket{11,g} 
\end{matrix}.\tag{22.17} $$
