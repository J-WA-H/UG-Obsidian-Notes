In experiments we have never directly observed a single quark, just hadrons. Consider the scattering of an electron of of a proton with $\sqrt{ s }\gg m_{p}\sim 1\text{ GeV}$. The electron can resolve the interior of the proton.
![[Pasted image 20260301121602.png]]
In this scattering, the electron scatters off of one of the up quarks, while the other quarks are unaffected.

This computation can be done two ways:
1. Parton model
2. Using most general tensors

First consider the parton model, compute the scattering $e^{-}+u\to e^- + u$. Calculate the partonic cross-section $d\hat{\sigma}$.
The matrix element is
$$-i\mathcal{M}=ie\bar{u}_{e}(k')\gamma^\mu u_{e}(k) \frac{{-ig_{\mu \nu}}}{q^2}\left( -i \frac{2}{3}e \right)\bar{u}_{u}(p')\gamma^{\nu}u_{u}(xp)\tag{8.1} $$
where $x$ is the fraction of the proton momentum given to the up quark in the interaction.
$$d\hat{\sigma}=\frac{1}{2} \frac{1}{2|\vec{k}|2x|\vec{p}|} \frac{d^3p'd^3k'}{(2\pi)^62|\vec{p}'|2|\vec{k}'|}|\mathcal{M}|^2(2\pi)^4\delta^{(4)}(xp-p'+k-k')\tag{8.2}. $$
First consider the phase space. For the quark phase space
$$(2\pi)^4\delta^{(4)}(xp+q-p') \frac{d^3p'}{(2\pi)^32|\vec{p}'|}=(2\pi)\delta(x|\vec{p}|+q^0-|\vec{p}'|) \frac{1}{2|x\vec{p}+\vec{q}|}=(2\pi)\delta(x|\vec{p}|+{q^0}-|x\vec{p}+\vec{q}|) \frac{1}{2|x\vec{p}+\vec{q}|}\tag{8.3}. $$
Using the identity $\delta(E-|\vec{p}|)=2|\vec{p}|\delta(E^2-p^2)\Theta(E)$, we can rewrite the $\delta$-function as
$$2|x\vec{p}+\vec{q}|\delta((x|\vec{p}|+q^0)^2-(x\vec{p}+\vec{q})^2)=2|x\vec{p}+\vec{q}|\delta((xp+q)^2)\tag{8.4} .$$
In the massless approximation this becomes
$$2\pi\delta(2p\cdot qx+q^2)\tag{8.5}. $$
Now consider the lepton phase space,
$$\frac{d^3k'}{(2\pi)^32E_{k'}}=\frac{|\vec{k}'|d|\vec{k}'|d\Omega}{2(2\pi)^3}=\frac{1}{2(2\pi)^2}|\vec{k}'|d|\vec{k}'|d\cos \theta \tag{8.6}. $$
Transform this to the Lorentz invariant quantities $(k',\cos \theta)\to(p\cdot q,q^2)$.
- $p\cdot q=p\cdot k-p\cdot k'=2|k|^2-|k||k'|(1+\cos \theta)$
- $q^2=-2k\cdot k'=-2|k||k'|(1-\cos \theta)$.

The Jacobian gives
$$J=\begin{vmatrix}
\frac{\partial q^2}{\partial |k'|} & \frac{\partial q^2}{\partial \cos \theta} \\
\frac{\partial(p\cdot q)}{\partial |k'|} & \frac{\partial(p\cdot q)}{d\cos \theta}
\end{vmatrix}=4|k|^2|k'|\tag{8.7} .$$
This gives
$$\frac{1}{8\pi^2}\cancel{|k'|} \frac{dq^2d(p\cdot q)}{4|k|^2\cancel{|k'|}}=\frac{1}{16\pi^2} \frac{dq^2d(p\cdot q)}{(p\cdot k)}\tag{8.8} $$
as in the COM frame $|k|^2=2p\cdot k$.

Now consider the matrix element,
$$|\overline{\mathcal{M}}|^2=\frac{1}{2^2}\sum_{spin}|\bar{u}_{e}\gamma_{\mu}u_{e} \frac{e^2}{q^2} \left( \frac{2}{3} \right)\bar{u}_{u}\gamma^{\mu}u_{u}|^2=\frac{1}{4}\left( \frac{2e^2}{3q^2} \right)\mathrm{Tr}[\gamma_{\mu}xp\!\!\!/\gamma_{\nu}p\!\!\!/']\mathrm{Tr}[\gamma^{\mu}k\!\!\!/\gamma^{\nu}k\!\!\!/']\tag{8.9}=\left( \frac{2e^2}{3q^2} \right)8(\underbrace{ (xp\cdot k)(p'\cdot k')+(xp\cdot k')(p'\cdot k) }_{ (xp\cdot k)^2+(xp\cdot k')^2 }). $$
This gives the partonic cross section,
$$d\hat{\sigma}=\left( \frac{2e^2}{3q^2} \right) \frac{1}{2(2p^0)(2k^0)}8x((p\cdot k)^2+(p\cdot k')^2) \frac{dq^2d(p\cdot k)}{16\pi^2(p\cdot k)}2\pi\delta(2xp\cdot q+q^2)\tag{8.10}. $$
The total cross-section is determined by the Parton distribution function (PDF),
$$d\sigma=d\hat{\sigma}f_{u}(x)dx\tag{8.11}. $$
From the $\delta$-function,
$$x=-\frac{q^2}{2p\cdot q}\tag{8.12}. $$
$$d\sigma=\left( \frac{2e^2}{3q^2} \right) \frac{p\cdot k}{4\pi} \left( 1+\frac{(p\cdot(k-q))^2}{(p\cdot k)^2} \right)d(p\cdot q)xf_{u}(x)dx\tag{8.13}=\frac{e^2}{8\pi} \frac{s}{q^4}\left( \frac{2e}{3} \right)^2(1+(1-y)^2)dyf_{u}(x)dx. $$
$y$ is the fraction of energy given to the proton,
$$y=\frac{{p\cdot q}}{p\cdot k}=\frac{2p^0q^0}{2p^0k^0}=\frac{q^0}{p^0}\tag{8.14}. $$
For the whole process,
$$d\sigma_{ep\to eX}=\frac{e^2}{8\pi} \frac{s}{q^4}(1+(1-y)^2)dy\left( \left( \frac{2e}{3} \right)^2f_{u}(x)+\left( -\frac{e}{3} \right)^2f_{d}(x) \right)xdx\tag{8.15}. $$
Consider the second method. Two generalised tensors are $L_{\mu \nu}$ (leptonic) and $W_{\mu \nu}$ (hadronic).
We can construct a symmetric $L_{\mu \nu}$ is
$$L_{\mu \nu}=2(k_{\mu}k'_{\nu}+k_{\nu}k_{\mu}'-g_{\mu \nu}k\cdot k')\tag{8.16} .$$
We now aim to construct a symmetric $W_{\mu \nu}$ from $g_{\mu \nu},p_{\mu}p_{\nu},q_{\mu}q_{\nu},p_{\mu}q_{\nu}+p_{\nu}q_{\mu}$. We know $q^\mu W_{\mu \nu}=0$ is a conserved current so
$$W_{\mu \nu}=F_{1}\left( -g_{\mu\nu}+\frac{q_{\mu}q_{\nu}}{q^2} \right)+F_{2}\left( p_{\mu}-\frac{p\cdot q}{q^2}q_{\mu} \right)\left( p_{\nu}-\frac{p\cdot q}{q^2}q_{\nu} \right)\tag{8.17} $$
is the only combination allowed. 

From this we can build $\sigma_{ep\to eX}$ from $L_{\mu \nu}W^{\mu \nu}$.
$$L_{\mu \nu}W^{\mu \nu}=F_{1}(-2q^2)+F_{2}(4(p\cdot k)(p\cdot k-p\cdot q))\tag{8.18} $$
To get a cross-section, we need a flux,
$$\frac{1}{4p\cdot k}=\frac{1}{2s}\tag{8.19}, $$
lepton phase space,
$$\frac{dq^2d(p\cdot q)}{(2\pi)^22s},\tag{8.20} $$
and a Jacobian
$$dq^2d(p\cdot q)=\frac{ys^2}{2}dxdy\tag{8.21} $$
which gives
$$d\sigma_{ep\to eX}=\frac{e^4}{4\pi q^4}s(xy^2F_{1}(x,y)+(1-y)F_{2}(x,y))dxdy\implies xy^2F_{1}+(1-y)F_{2}=\frac{1}{2}(1+(1-y)^2)\sum_{i}Q_{i}^2f_{i}\tag{8.22} $$
$$\implies F_{2}(x,y)=2xF_{1}(x,y)=\sum_{i}Q_{i}^2f_{i}(x)\tag{8.22} .$$
This is the Callan-Gross relation. We also get
$$F_{i}(x,y)=F_{i}(x)\tag{8.23} .$$
This is Bjorken scaling. This matches experiment so confirms the parton model.

$xf_{u}(x)$ peaks at $x=\frac{1}{3}$ but does not vanish at small $x$. If $xf_{u}(x)\sim \text{const}$, $f_{i}\sim \frac{1}{x}\implies \int_{0}^{1}fdx$ diverges, so the model of the proton as 3 quarks is not correct.
![[Pasted image 20260308180629.png]]
The top diagram shows [[QCD]] interactions between quarks via gluons and the bottom one shows virtual gluon emission giving a $q\bar{q}$ pair.
The PDFs for these are
![[Pasted image 20260308180955.png]]
![[Pasted image 20260308181053.png]]
These show protons are made of:
- Valance quarks $(uud)$
- sea quarks $(q\bar{q})$
$$\int_{0}^{1}f_{u}(x)-f_{\bar{u}}(x)dx=2,\qquad \int_{0}^{1}f_{d}(x)-f_{\bar{d}}(x)dx=1\tag{8.24}. $$
The total,
$$\int\left[ \sum_{i\in\text{partons}}f_{i}(x) \right]dx=1\tag{8.25}. $$
with all $q,\bar{q}\to \frac{1}{2}$, which shows there is something in the proton that hasn't been accounted for (gluons).

At the LHC, the collision of 2 protons has
$$\sigma(s)=\sum_{ij}\int dx_{1}dx_{2}f_{i}(x_{1})f_{j}(x_{2})\hat{\sigma}_{ij}(x_{1},x_{2},s)\tag{8.26}. $$
with
$$s=(p+k)^2\approx 2p\cdot k,\qquad \hat{s}=(x_{1}p+x_{2}k)^2=x_{1}x_{2}s\tag{8.27}. $$
