For simplicity we will consider the domain and codomain will be the same, with [basis](Basis%20of%20Vectors.md) $B=\{\underline{e}_{j}\}$. The [operator](Linear%20Operators.md) $A$ in this basis has components $A^i_{\;j}$. For a change of basis to $B'=\{\underline{e}_{j}'\}$, we use a [coordinate transform](Coordinate%20Transforms.md) 
$$\underline{e}_{j}'=\underline{e}_{i}S^{\;i}_{j}.$$
$$\underline{x}'^{j}=(S^{-1})^j_{\;i}x^{i}=R^j_{\;i}x^i.$$
For a vector in the original basis $\underline{y}=A\underline{x}$, $y^i=A^j_{\;i}x^i$, and in the new basis $y'^j=A'^j_{\;i}x'^i$.
$$y^j=A^j_{\;i}x^i$$
$$S^{j}_{\;k}y'^k=A^j_{\;i}S^{i}_{\;l}x'^l$$
$$y'^k=(S^{-1})^k_{\;j}A^j_{\;i}S^{i}_{\;l}x'^{l}$$
$$\implies A'^k_{\;l}=(S^{-1})^{k}_{\;j}A^{j}_{\;i}S^{i}_{\;l}.$$
In matrix notation:
$$A'=S^{-1}AS.$$
