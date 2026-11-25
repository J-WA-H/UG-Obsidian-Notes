To go from SR $\to$ GR: when you see a Minkowski metric, replace it with a more general metric: $$\eta^{\alpha\beta} \;\longrightarrow\; g^{\alpha\beta}\tag{10.1} $$ Also, when we have $\partial_\mu$, replace with the covariant derivative (comma-to-semicolon rule): $$\partial_\mu \;\longrightarrow\; ;e \tag{10.2} $$ > Note: $\partial_\mu x^\nu \mapsto \dfrac{\partial x^\nu}{\partial x^\alpha}\dfrac{\partial x^\alpha}{\partial x^\mu}$ **Example** the [[Stress-Energy Tensor]]:
$$T^{\mu\nu} = \left(\rho_0 + \frac{P}{c^2}\right)u^\mu u^\nu - P\,\eta^{\mu\nu} \;\longrightarrow\; T^{\mu\nu} = \left(\rho_0 + \frac{P}{c^2}\right)u^\mu u^\nu - P\,g^{\mu\nu}\tag{10.3} $$
$$\partial_\nu T^{\mu\nu} = 0 \;\longrightarrow\; T^{\mu\nu}{}_{;\nu} = 0\tag{10.4}$$
Einstein's equations relate gravity to curvature: $$T^{\mu\nu} \longleftrightarrow R^\alpha{}_{\beta\gamma\delta}\tag{10.5} $$ - LHS: $2^{\text{nd}}$-order tensor - RHS: $4^{\text{th}}$-order tensor We could contract the $4^{\text{th}}$-order tensor to a $2^{\text{nd}}$-order tensor, but contraction loses some information. However, $R^\alpha{}_{\beta\gamma\delta}$ only has $n^2(n^2-1)/12$ independent components, so we don't lose as much information. We need to choose which bottom index to contract over: $R^a{}_{acd}$, $R^a{}_{bad}$, or $R^a{}_{bca}$. **Index symmetries:** $R_{abcd} = g_{ae} R^a{}_{bcd}$ 
$$R_{abcd} = -R_{bacd}\tag{10.6} $$
$$\therefore \quad R_{aacd} = -R_{aacd} \;\Rightarrow\; R_{aacd} = 0 \quad \text{— don't choose the first (covariant) index}\tag{10.7} $$
$$R_{abcd} = -R_{abdc} \quad \text{(doesn't matter if we contract over } c \text{ or } d \text{, just need to account for negative sign)}\tag{10.8} $$
$$R^a{}_{bad} = -R^a{}_{bda}\tag{10.9} $$
Choose to sum over the **last** index. **Define the Ricci tensor:** $$R_{ab} \equiv R^c{}_{acb}\tag{10.10} $$ **Try** $R^{\mu\nu} = \kappa\, T^{\mu\nu}$ We know $T^{\mu\nu}$ is symmetric and $T^{\mu\nu}{}_{;\nu} = 0$ (and $T^{\mu\nu} = T^{\nu\mu}$). Check these hold for $R^{\mu\nu}$. ### Symmetries — Cyclic Identity $$R^a{}_{bcd} + R^a{}_{cdb} + R^a{}_{dbc} = 0\tag{10.11} $$ Setting $a = d$: 
$$R^a{}_{bca} + R^a{}_{cab} + R^a{}_{abc} = 0\tag{10.12} $$
$$R_{bc} - R^a{}_{cba} + R^a{}_{abc} = 0 \;\Rightarrow\; R_{bc} - R_{cb} = 0 \;\Rightarrow\; R_{bc} = R_{cb}\tag{10.13} $$
$$\therefore \quad \text{Ricci tensor is symmetric.}$$
In a local geodesic frame (Christoffel symbols zero, but derivatives are not): $$R^a{}_{bcd} = \partial_c\,\Gamma^a{}_{bd} - \partial_d\,\Gamma^a{}_{bc}\tag{10.14} $$ In this frame $\nabla_e = \partial_e$, so: 
$$\nabla_e R^a{}_{bcd} = \partial_e\left(\partial_c\,\Gamma^a{}_{db} - \partial_d\,\Gamma^a{}_{cb}\right) = \partial_e\partial_c\,\Gamma^a{}_{db} - \partial_e\partial_d\,\Gamma^a{}_{cb}\tag{10.15} $$
$$R^a{}_{bde;c} = \partial_c\partial_d\,\Gamma^a{}_{cb} - \partial_c\partial_e\,\Gamma^a{}_{db}\tag{10.16} $$
$$R^a{}_{bec;d} = \partial_d\partial_e\,\Gamma^a{}_{cb} - \partial_d\partial_c\,\Gamma^a{}_{eb}\tag{10.17} $$
Adding all three: $$R^a{}_{bcd;e} + R^a{}_{bde;c} + R^a{}_{bec;d} = 0 \qquad \textbf{— Bianchi identity}\tag{10.18} $$Contract over $a$ 
$$R^a{}_{bca;e} + R^a{}_{bae;c} + R^a{}_{bec;a} = 0\tag{10.19} $$
$$R_{bc;e} - R_{be;c} + R^a{}_{bec;a} = 0\tag{10.20} $$
Since $g_{ab;c} = 0$ by definition, we can raise/lower indices freely: 
$$\lambda_{a;c} = (g_{ab}\lambda^b)_{;c} = g_{ab;c}\lambda^b + g_{ab}\lambda^b{}_{;c} = g_{ab}\lambda^b{}_{;c}\tag{10.21} $$
$$\therefore \quad g^{fb}R_{bc;e} - g^{fb}R_{be;c} + g^{fb}R^a{}_{bec;a} = 0\tag{10.22} $$
$$R^f{}_{c;e} - R^f{}_{e;c} + R^{af}{}_{ec;a} = 0\tag{10.23} $$
Contract over $e = f$ $$R^e{}_{c;e} - R^e{}_{e;c} + R^{ae}{}_{ec;a} = 0\tag{10.24} $$ **Define** $R^a{}_a \equiv R$ as the **Riemann curvature scalar**. 
$$R^e{}_{c;e} - R_{;c} + R^a{}_{ca;a} = 0 \quad (e, a \text{ are dummy indices, let } e \to a)\tag{10.25} $$
$$2R^a{}_{ca} = R_{;c}\tag{10.26} $$
$$R^a{}_{c;a} = \frac{1}{2}R_{;c}\tag{10.27} $$
$$\left(R^b{}_c - \frac{1}{2}R\,\delta^b{}_c\right)_{;b} = 0\tag{10.28} $$
$$\left(g^{ac}R^b{}_c - \frac{1}{2}R\,g^{ac}\delta^b{}_c\right)_{;b} = 0\tag{10.29} $$
$$\left(R^{ba} - \frac{1}{2}g^{ab}R\right)_{;b} = 0\tag{10.30} $$
$$\Rightarrow \quad R^{ba}{}_{;b} = \frac{1}{2}g^{ab}R \neq 0\tag{10.31} $$
$\therefore \quad R^{\mu\nu} \neq \kappa\,T^{\mu\nu}$ This can be modified so both sides have zero covariant derivative. $R^{ba} - \frac{1}{2}g^{ab}R$ is a $2^{\text{nd}}$-order, symmetric tensor with ${}_{;b} = 0$. Now try: 
$$\boxed{R^{\mu\nu} - \frac{1}{2}g^{\mu\nu}R = \kappa\,T^{\mu\nu}} \qquad \textbf{Einstein equation}\tag{10.32} $$
More generally, we need an integration constant,
$$R^{\mu \nu}-\frac{1}{2}g^{\mu \nu}R+\Lambda g^{\mu \nu}=\kappa T^{\mu \nu}\tag{10.33}. $$
This turns out to be the cosmological constant. Assume $\Lambda\cong 0$ for black holes as the size scale is so tiny that approximating the universe as static is valid.

We can rearrange the Einstein field equations into a form easier to use.
$$g_{\gamma \nu}\left( R^{\mu \nu}-\frac{1}{2}g^{\mu \nu}R \right)=\kappa g_{\gamma \mu}T^{\mu \nu}\tag{10.34} \implies R_{\gamma}\\^{\nu}-\frac{1}{2}g_{\gamma \mu}g^{\mu \nu}R=\kappa T_{\gamma}\\^{\nu}\implies R_{\gamma}\\^{\nu}-\frac{1}{2}\delta_{\gamma}\\^{\nu}R=\kappa T_{\gamma}\\^{\nu}.$$
Let $\gamma=\nu$, 
$$R_{\gamma}\\^{\gamma}-\frac{4}{2}R=\kappa T_{\gamma}\\^{\gamma}\implies R=-\kappa T\tag{10.35} $$
This gives
$$R^{\mu \nu}=\kappa\left( T^{\mu \nu}-\frac{1}{2}g^{\mu \nu}T \right)\tag{10.36}. $$
