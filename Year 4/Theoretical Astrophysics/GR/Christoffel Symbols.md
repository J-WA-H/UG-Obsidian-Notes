Using the definition of the [basis vector](Tensors%20and%20Metrics.md), and [Christoffel symbol](Parallel%20Transport.md)
$$\vec{e}_{a}=\frac{\partial \vec{r}}{\partial x^a},\;\Gamma^c_{\;ab}\vec{e}_{c}=\frac{\partial \vec{e}_{a}}{\partial x^b}\tag{5.1} .$$
$$\frac{\partial \vec{e}_{a}}{\partial x^b}=\frac{\partial}{\partial x^b}\left( \frac{\partial \vec{r}}{\partial x^a} \right)=\frac{\partial^2\vec{r}}{\partial x^b\partial x^a}=\frac{\partial^2\vec{r}}{\partial x^a\partial x^b}=\frac{\partial}{\partial x^a}\left( \frac{\partial \vec{r}}{\partial x^b} \right)=\frac{\partial \vec{e}_{b}}{\partial x^a}\tag{5.2} $$which shows the Christoffel symbol is symmetric with respect to its bottom two indices $\Gamma^c_{\;ab}=\Gamma^c_{\;ba}$.
$$\frac{\partial g_{bc}}{\partial x^c}=\frac{\partial(\vec{e}_{a}\cdot \vec{e}_{b})}{\partial x^c}=\frac{\partial \vec{e}_{a}}{\partial x^c}\cdot \vec{e}_{b}+\vec{e}_{a} \frac{\partial \vec{e}_{b}}{\partial x^c}=\Gamma^d_{\;ac}\vec{e}_{d}\cdot \vec{e}_{b}+\vec{e}_{a}\cdot\Gamma^d_{\;bc}\vec{e}_{d}=\Gamma^d_{\;ac}g_{ab}+g_{ad}\Gamma^d_{\;bc}\tag{5.3} $$
$$\frac{\partial g_{bc}}{\partial x^a}=\Gamma^d_{\;ba}g_{dc}+g_{bd}\Gamma^d_{\;ca}\tag{5.4} $$
$$\frac{\partial g_{ca}}{\partial x^b}=\Gamma^d_{\;cb}g_{da}+g_{cd}\Gamma^d_{\;ab}.\tag{5.5} $$Adding $(5.3)$ and $(5.4)$, and subtracting $(5.5)$ gives
$$\frac{\partial g_{ab}}{\partial{x^c}}+\frac{\partial g_{bc}}{\partial x^a}-\frac{\partial g_{ca}}{\partial x^b}=\Gamma^d_{\;ac}+\cancel{g_{ab}\Gamma^d_{\;bc}}+\cancel{\Gamma^d_{\;ba}g_{dc}}+g_{bd}\Gamma^d_{\;ca}-\cancel{\Gamma^d_{\;^{3}}g_{da}}-\cancel{g_{cd}\Gamma^d_{\;ab}}=2\Gamma^d_{\;ac}g_{db}\tag{5.6} .$$
Multiplying both sides by $\frac{1}{2}g^{fb}$ gives
$$\Gamma^b_{\;ca}=\frac{1}{2}g^{fb}\left(\frac{\partial g_{ab}}{\partial{x^c}}+\frac{\partial g_{bc}}{\partial x^a}-\frac{\partial g_{ca}}{\partial x^b}\right)\tag{5.7} .$$
This can be used to describe surfaces, for example a 2D sphere,
$$ds^2=dx^2+dy^2\tag{5.8} ;\;g_{AB}=\mathrm{diag}(1,1).$$
since $g_{AB}$ does not depend on the coordinates, $\Gamma^A_{\;BC}=0$.

Now consider the surface of a sphere of fixed radius $a$,
$$ds^2=a^2d\theta^2+a^2\sin^2\theta d\phi^2\tag{5.9} ;\;g_{AB}=\mathrm{diag}(a^2,a^2\sin^2\theta).$$
To find the Christoffel symbol, we need to find the contravariant metric using the identity $g_{AB}g^{BC}=\delta_{A}^{\;C}$.
$$g_{1B}g^{B{1}}=\delta_{1}^{\;1}=1=g_{11}g^{11}+\cancelto{0}{g_{12}}g^{21}=g_{11}g^{11}=a^2g^{11}\implies g^{11}=\frac{1}{a^2}.\tag{5.10} $$
$$g_{1B}g^{B 2}=\delta_{1}^{\;2}=0=g_{11}g^{12}+\cancelto{0}{g_{12}}g^{22}=g_{11}g^{12}=a^2g^{12}\implies g^{12}=0\tag{5.11} $$ $$g_{2B}g^{B 2}=\delta_{2}^{\;2}=1=\cancelto{0}{g_{21}}g^{12}+g_{22}g^{22}=g_{22}g^{22}=a^2\sin^2\theta g^{22}=1\implies g^{22}=\frac{1}{a^2\sin^2\theta}\tag{5.12} $$ $$g_{2B}g^{B 1}=\delta_{2}^{\;1}=0=\cancelto{0}{g_{21}}g^{11}+g_{22}g^{21}=g_{22}g^{21}=a^2\sin^2\theta g^{21}\implies g^{21}=0.$$This gives the contravariant metric 
$$g^{AB}=\mathrm{diag}\left( \frac{1}{a^2}, \frac{1}{a^2\sin^2\theta} \right).\tag{5.13} $$
Iff we have a diagonal metric, $g^{aa}=\frac{1}{g_{aa}}$ and $g^{ab}=0$.
To find the Christoffel symbol,
$$\Gamma^1_{\;11}=\Gamma^\theta_{\;\theta \theta}=\frac{1}{2}g^{1B}(\partial_{1}g_{1B}+\partial_{1}g_{B{1}}-\partial_{B}g_{11})=\frac{1}{2}g^{11}(\partial_{1}g_{11}+\partial_{1}g_{11}-\partial_{1}g_{11})=0.\tag{5.14} $$
$$\Gamma^1_{\;22}=\frac{1}{2}g^{1B}(\partial_{2}g_{2B}+\partial_{2}g_{B{2}}-\partial_{B}g_{22})=\frac{1}{2}g^{11}(\partial_{2}g_{21}+\partial_{2}g_{12}-\partial_{1}g_{22})=-\frac{1}{2} \frac{1}{a^2}a^22\sin \theta \cos \theta=-\frac{1}{2}\sin{2}\theta.\tag{5.15} $$
$$\Gamma^2_{\;12}=\frac{1}{2}g^{2B}(\partial_{1}g_{2B}+\partial_{2}g_{B{2}}-\partial_{B}g_{12})=\frac{1}{2}g^{22}(\partial_{1}g_{22}+\partial_{2}g_{22}-\partial_{2}g_{22})=\frac{1}{2}g^{22}\partial_{1}g_{22}=\frac{1}{a^2\sin ^2\theta}a^2\sin \theta \cos \theta=\cot \theta.\tag{5.16} $$
