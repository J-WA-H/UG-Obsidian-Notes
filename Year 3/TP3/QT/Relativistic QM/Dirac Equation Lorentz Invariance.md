We have a [[Covariant Form of the Dirac Equation]] as
$$\left( i\partial \!\!\!/-\frac{mc}{\hbar} \right)\psi(\underline{x},t)=0.$$
This looks like it might be covariant as space and time are on the same footing - but $\gamma^{\mu}$ isn't a normal 4-component object.
$$\gamma^{0}=\begin{bmatrix}
0 & \mathbb{I}_{2} \\
\mathbb{I}_{2} & 0
\end{bmatrix};\;\gamma^{k}=\begin{bmatrix}
0 & \sigma^{k} \\
-\sigma^{k} & 0
\end{bmatrix}.$$
We don't expect these to be a 4-vector - so we don't expect it to transform under a [Lorentz Transformation](Index%20and%20Tensor%20Notation.md) so the $\gamma$ matrices are Lorentz invariant.

Think about how the system changes under a Lorentz transformation. Consider how the [Dirac spinor](Dirac%20Equation%20Derivation.md) transforms so the Dirac equation is valid in all inertial frames.

We need to allow the spinor to transform between frames. As the spinor is a 4D vector, the Lorentz transform must be a 4x4 matrix,
$$x'=\Lambda x$$
$$\psi'(x')=S(\Lambda)\psi(x).$$
The matrix $S(\Lambda)$ depends on the specific Lorentz transform.

Consider 2 frames, $I$ with 4-position $x^{\mu}$ and spinor $\psi(x)$, and $I'$ with 4-position $x'^{\mu}$ and spinor $\psi'(x')$.
In frame $I$:
$$\left( -i\gamma^{\mu}\partial_{\mu}+\frac{mc}{\hbar} \right)\psi(x)=0$$
$$\partial_{\mu}=\Lambda^{\mu}_{\;\nu}\partial'_{\nu}.$$
$$\psi(x)=S^{-1}(\Lambda)\psi'(x').$$
Substituting these into the Dirac equation gives
$$\left( -\gamma^{\mu}\Lambda^{\nu}_{\;\mu}\partial'_{\nu}+{\frac{mc}{\hbar}} \right)S^{-1}(\Lambda)\psi'(x')=0.$$
Left multiply by $S(\Lambda)$,
$$\left( -iS(\Lambda)\gamma^{\mu}\Lambda^{\nu}_{\;\mu}S^{-1}(\Lambda)\partial'_{\nu}+\frac{mc}{\hbar} \right)\psi'(x')=0.$$
The Dirac equation is invariant if
$$S(\Lambda)\gamma^{\mu}S^{-1}(\Lambda)\Lambda^{\mu}_{\;\nu}=\gamma^{\nu}.$$
$\Lambda^{\mu}_{\;\nu}$ was brought to the left as it is not in spinor space so $S(\Lambda)$ and $\gamma$ don't act on it.
Left multiplying by $S^{-1}(\Lambda)$ and right multiply by $S(\Lambda)$
$$\gamma^{\mu}\Lambda^{\mu}_{\;\nu}=S^{-1}(\Lambda)\gamma^{\nu}S(\Lambda).$$
This determines the form of $S(\Lambda)$, analogous to how $g=\Lambda^{T}g\Lambda$ for the metric defines the form of $\Lambda$.
The main examples are [[Rotations]] and boosts,
Example: Rotation about $z$:
$$R_{12}=\begin{bmatrix}
1 & 0 & 0 & 0 \\
0 & \cos \phi & \sin \phi & 0 \\
0 & -\sin \phi & \cos \phi & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}.$$
$$\therefore S(R_{12})=\begin{bmatrix}
\cos \phi+i\sin \phi & 0 & 0 & 0 \\
0 & \cos \phi-i\sin \phi & 0 & 0 \\
0 & 0 & \cos \phi+i\sin \phi & 0 \\
0 & 0 & 0 & \cos \phi-i\sin \phi
\end{bmatrix}.$$This shows that for spinors, we need a rotation of $4\pi$ to return to its original value.

Example: Boost along $x$ axis
$$L_{01}=\begin{bmatrix}
\cosh \eta & -\sinh \eta & 0 & 0 \\
-\sinh \eta & \cosh \eta & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}.$$
$$\therefore S(L_{01})=\begin{bmatrix}
\cosh \eta & 0 & 0 & \sinh \eta \\
0 & \cosh \eta & \sinh \eta & 0 \\
0 & \sinh \eta & \cosh \eta & 0 \\
\sinh \eta & 0 & 0 & \cosh \eta
\end{bmatrix}.$$
