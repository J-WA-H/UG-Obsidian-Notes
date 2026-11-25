To solve the Schrodinger-like equation in the [[Born-Oppenheimer Approximation]], we note that
$$|\Psi_{a}(\vec{r},\vec{r}')|^2=\frac{1}{2}[|\phi_{1}(\vec{r})|^2+|\phi_{2}(\vec{r})|^2][|\phi_{1}(\vec{r}')|^2+|\phi_{2}(\vec{r}')|^2]+\frac{1}{2}[\phi_{1}(\vec{r})\phi_{1}^{*}(\vec{r}')+\phi_{2}(\vec{r})\phi_{2}^{*}(\vec{r}')][\phi_{1}^{*}(\vec{r})\phi_{1}(\vec{r}')+\phi_{2}^{*}(\vec{r})\phi_{2}(\vec{r}')]\tag{3.1}. $$
This is equivalent to
$$\frac{1}{2}\rho(\vec{r})\rho(\vec{r}')-\frac{1}{2}\rho (\vec{r},\vec{r}')\rho(\vec{r}',\vec{r})\tag{3.2} .$$
$\rho(\vec{r})$ is the density of fermions and $\rho(\vec{r},\vec{r}')$ is the one-body reduced density matrix.
$$\rho(\vec{r})=\sum _{i=1}^N|\phi_{i}(\vec{r})|^2,\;\rho(\vec{r},\vec{r}')=\sum_{i=1}^N\phi_{i}(\vec{r})\phi ^{*}_{i}(\vec{r}')\tag{3.3}. $$
For spin $\sigma$,
$$\rho^\sigma(\vec{r})=\sum_{i=1}^{N^\sigma}|\phi_{i}^\sigma(\vec{r})|^2,\;\rho (\vec{r})=\sum_{\sigma=\uparrow\downarrow}\rho^\sigma(\vec{r}).\tag{3.4} $$
The N-body, non-reduced density matrix is
$$\Gamma(\vec{r}_{1},\dots \vec{r}_{N};\vec{r}_{1}',\dots,\vec{r}_{N}')=\psi(\vec{r}_{1},\dots,\vec{r}_{N})\psi ^{*}(\vec{r}_{1}',\dots,\vec{r}_{N}')\tag{3.5}. $$The reduced density matrix is then
$$\rho(\vec{r}_{1},\vec{r}_{1}')=N\int dr_{2}\dots dr_{N}\delta(r_{2}-r_{2}')\dots\delta(r_{N}-r_{N}')\Gamma(\vec{r}_{1},\dots,\vec{r}_{N};\vec{r}_{1}',\dots,\vec{r}_{N}')\tag{3.6} $$$$\gamma_{2}(\vec{r}_{1},\vec{r}_{2};\vec{r}_{1}',\vec{r}_{2}')=\frac{N(N-1)}{2}\int dr_{3}\dots \int dr_{N}\Gamma(\vec{r}_{1},\dots,\vec{r}_{N};\vec{r}_{1}',\dots \vec{r}_{N}')\tag{3.7}.$$If we have the [Slater determinant](Two%20electron%20atoms.md) $\Phi=\frac{1}{N!}\begin{vmatrix}\phi_{1}^\uparrow ,\phi_{2}^\uparrow,\dots,\phi_{N}^\uparrow;\phi_{1}^\downarrow,\dots ,\phi_{N}^\downarrow \end{vmatrix}$,
$$\rho^\sigma(\vec{r})=\sum_{i=1}^{N^\sigma}|\phi_{i}^\sigma(\vec{r})|^2;\;\;\rho^\sigma(\vec{r},\vec{r}')=\sum_{i=1}^{N^\sigma}\phi_{i}(\vec{r})\phi_{i}^{\sigma*}(\vec{r}')\tag{3.8} $$which gives
$$\gamma_{2}=\frac{1}{2}\rho(\vec{r})\rho(\vec{r}')-\sum_{\sigma} \frac{1}{2}\rho^\sigma(\vec{r},\vec{r}')\rho^\sigma(\vec{r}',\vec{r}).$$
Note
$$\bra{\psi} V\ket{\psi} =\int d^3r\rho(\vec{r})V(\vec{r})\tag{3.9} $$
$$\bra{\psi} T\ket{\psi} =\sum_{\sigma}\iint d^3r d^3r'\delta^{(3)}(\vec{r}-\vec{r}')\left[ \left( -\frac{\nabla^2}{2} \right)\rho^{\sigma}(\vec{r},\vec{r}') \right]\tag{3.10} .$$
