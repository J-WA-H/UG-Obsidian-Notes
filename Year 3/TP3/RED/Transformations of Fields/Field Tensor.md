We have derived how EM field [transform](EM%20Lorentz%20Transformations.md):
$$E_{x}'=E_{x};\;\;B_{x}'=B_{x}$$
$$E_{y}'=\gamma(E_{y}-vB_{z});\;\;B_{y}'=\gamma\left( B_{y}+\frac{v}{c^2}E_{z} \right)$$
$$E_{z}'=\gamma(E_{z}+vB_{y});\;\;B_{z}'=\gamma\left( B_{z}-\frac{v}{c^2}E_{y} \right).$$
The field tensor $F^{\mu \nu}$ transforms EM fields subject to these transformations.
$$t^{\mu \nu}\to t'^{\mu \nu}=\Lambda^{\mu}_{\;\sigma}\Lambda^{\nu}_{\;\rho}t^{\sigma \rho}.$$
Rank-2 tensors have 16 elements but the field transformation only has 6 so we have to impose some conditions.
We will use an anti-symmetric tensor:
Properties:
- $$t^{\mu \nu}=-t^{\nu \mu}.$$
- Elements of the lower triangle are the same as the upper triangle by with a minus sign
- All diagonal elements are 0
$$t'^{01}=\Lambda^{0}_{\;\lambda}\Lambda^{1}_{\;\sigma}t^{\lambda\sigma}=(\Lambda^{0}_{\;0}\Lambda^{1}_{\;1}-\Lambda^{0}_{\;1}\Lambda^{1}_{\;0})t^{01}$$
these are the only non-zero relevant elements in the [Lorentz transformation matrix](4-Vectors.md). Expanding this gives
$$t'^{01}=(\gamma^2-\gamma^2\beta^2)t^{01}=\gamma^2(1-\beta^2)t^{01}=t^{01}.$$
Doing this for all elements in the upper triangle of the $t^{\mu \nu}$ tensor gives
$$t'^{01}=t^{01};\;\;t'^{12}=\gamma(t^{12}-\beta t^{02})$$
$$t'^{02}=\gamma(t^{02}-\beta t^{12});\;\;t'^{13}=\gamma(t^{13}-\beta t^{03})$$
$$t'^{03}=\gamma(t^{03}-\beta t^{13});\;\;t'^{23}=t^{23}.$$
Using these relations with the field transformations gives the field tensor
$$F^{\mu \nu}=\begin{bmatrix}
0 & -E_{x} & -E_{y} & -E_{z} \\
E_{x} & 0 & -cB_{z} & cB_{y} \\
E_{y} & cB_{z} & 0 & -cB_{x} \\
E_{z} & -cB_{y} & cB_{x} & 0
\end{bmatrix}.$$
The dual field tensor also gives the same transformation of EM fields, given by
$$\tilde{F}^{\mu \nu}=\begin{bmatrix}
0 & cB_{x} & cB_{y} & cB_{z} \\
-cB_{x} & 0 & -E_{z} & E_{y} \\
-cB_{y} & E_{z} & 0 & -E_{x} \\
-cB_{z} & -E_{y} & E_{x} & 0
\end{bmatrix}.$$
Invariant quantities are the product of two field tensors
$$F^{\mu \nu}F_{\mu \nu}=-F^{\mu \nu}F_{\nu \mu}=-2(E^2-c^2B^2).$$
This shows that if $E>B$ in one frame, then $E>B$ in all frames.
$$F_{\mu \nu}\tilde{F}^{\mu \nu}=-4c\underline{E}\cdot \underline{B}.$$
This shows that if $\underline{E}$ is orthogonal to $\underline{B}$ in one frame, they are orthogonal in all frames.
Since the metric is symmetric and the field tensor is anti-symmetric, their product is zero.
$$g_{\mu \nu}F^{\mu \nu}=0.$$
