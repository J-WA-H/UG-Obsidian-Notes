Classically, when a magnetic moment is placed in a magnetic field it processes with a frequency
$$\omega_{L}=-\gamma B$$
where $\omega_{L}$ is the Larmor frequency and $\gamma$ is the gyroscopic ratio. For an electron, 
$$\gamma=-\frac{g_{s}\mu_{B}}{\hbar};\;g_{s}=2;\;\mu_B=\frac{e\hbar}{2m_{e}}.$$
The magnetic moment is given by $$\underline{\mu}=\gamma \underline{\hat{S}}.$$
And the total energy is given by
$$E=-\underline{\mu}\cdot \underline{B}$$
In this case we will take $\underline{B}$ to be along the z axis, $\underline{B}=B \underline{\hat{z}}$.
The total energy thus gives us the Hamiltonian of the system for a spin-1/2 particle:
$$\hat{H}=-\underline{\mu}\cdot \underline{B}=-\underline{\mu}\cdot B\underline{\hat{z}}=-\gamma B\hat{S}_{z}=\frac{\omega_{L}\hbar}{2}\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}.$$
The [spin states](Spin.md) are thus eigenfunctions of this Hamiltonian so we can use this to determine the eigenenergies:
$$\hat{H}\chi_{\uparrow}=E_{\uparrow}\chi_{\uparrow}$$
$$\frac{\omega_{L}\hbar}{2}\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}\begin{bmatrix}
1 \\
0
\end{bmatrix}=\frac{\omega_{L}\hbar}{2}\begin{bmatrix}
1 \\
0
\end{bmatrix}$$
$$\implies E_{\uparrow}=\frac{\omega_{L}\hbar}{2}.$$
$$\hat{H}\chi_{\downarrow}=E_{\downarrow}\chi_{\downarrow}$$
$$\frac{\omega_{L}\hbar}{2}\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}\begin{bmatrix}
0 \\
1
\end{bmatrix}=-\frac{\omega_{L}\hbar}{2}\begin{bmatrix}
0 \\
1
\end{bmatrix}$$
$$\implies E_{\downarrow}=-\frac{\omega_{L}\hbar}{2}.$$
These eigenstates can now be used to determine the time evolution of the spin states.
$$\chi(t=0)=\begin{bmatrix}
a \\
b
\end{bmatrix}=a\begin{bmatrix}
1 \\
0
\end{bmatrix}+b\begin{bmatrix}
0 \\
1
\end{bmatrix}.$$
Since this spin state must be normalised, we know that $a=\cos\left( \frac{\alpha}{2} \right)$ and $b=\sin\left( \frac{\alpha}{2} \right)$.
We know the time dependence of a quantum state with a time independent Hamiltonian is $\exp\left[ -\frac{iE}{\hbar}t \right]$, so 
$$\chi(t)=\cos\left( \frac{\alpha}{2} \right)\begin{bmatrix}
1 \\
0
\end{bmatrix}e^{-i \omega_{L}t/2}+\sin\left( \frac{\alpha}{2} \right)\begin{bmatrix}
0 \\
1
\end{bmatrix}e^{i\omega_{L}t/\hbar}.$$
$$=\begin{bmatrix}
\cos\left( \frac{\alpha}{2} \right)e^{-i\omega_{L}t/2} \\
\sin\left( \frac{\alpha}{2} \right)e^{i\omega_{L}t/2}
\end{bmatrix}.$$
