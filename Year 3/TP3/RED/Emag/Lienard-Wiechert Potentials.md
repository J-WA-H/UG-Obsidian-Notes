Consider the instantaneous rest frame of the particle.
We are only considering one point charge so 
$$\phi(\underline{r},t)=\frac{q}{4\pi\varepsilon_{0}\lvert \underline{R}' \rvert }=\frac{e}{\lvert \underline{R}' \rvert }$$
where $e=\frac{q}{4\pi\varepsilon_{0}}$.
As we are in the instantaneous rest frame, there is no current so $\underline{j}=\underline{0}$ so $\underline{A}=\underline{0}$.

We will now find the [[4-Potential]], which should involve distance and the [[4-Velocity]].

We can propose
$$A^\mu=\frac{eu^\mu}{u_{\nu}R^{\nu}}$$
where $R^\nu=r^\nu-r'^\nu$.
In the rest frame of the particle, $u^\mu=(c,\underline{0})$, $R^\nu=(c(t-t_{r}),\underline{R})$.
$$R_\nu R^\nu=c^2(t-t_{r})^2-\lvert \underline{R} \rvert^2=0 $$
from the definition of the [retarded time](Fields%20of%20a%20moving%20point%20charge.md), $\lvert \underline{R} \rvert=c(t-t_{r})$.
$$u_{\nu}R^\nu=c^2(t-t_r)=c\lvert \underline{R} \rvert. $$
$$A^\mu=\frac{eu^\mu}{u_{\nu}R^\nu}=\left( \frac{e}{\lvert \underline{R} \rvert },\underline{0} \right).$$
In the frame where the particle moves at speed $v$,
$$u_{\nu}R^\nu=\begin{bmatrix}
\gamma c & -\gamma \underline{v}
\end{bmatrix}\begin{bmatrix}
c(t-t_{r}) \\
\underline{R}
\end{bmatrix}=\gamma c\left( \lvert \underline{R} \rvert-\frac{{\underline{v}\cdot \underline{R}}}{c}  \right)=\gamma c(\lvert \underline{R}-\underline{\beta}\cdot \underline{R} \rvert ).$$
$$A^\mu=\frac{eu^\mu}{u_{\nu}R^\nu}=\left( \frac{e}{\lvert \underline{R} \rvert-\underline{\beta}\cdot \underline{R} }, \frac{e\underline{\beta}}{\lvert \underline{R} \rvert-\underline{\beta}\cdot \underline{R} } \right).$$
This gives
$$\phi(\underline{r},t)=\frac{e}{\lvert \underline{R} \rvert-\underline{\beta}\cdot \underline{R} };\;\underline{A}(\underline{r},t)=\frac{e\underline{\beta}}{c(\lvert \underline{R} \rvert-\underline{\beta}\cdot \underline{R} )}.$$
Using these potentials we get the physical fields:
$$\underline{E}=\frac{q}{4\pi\varepsilon_{0}} \frac{R}{(\underline{R}\cdot \underline{u})^3}[(c^2-v^2)\underline{u}+\underline{R}\times(\underline{u}\times \underline{a})]$$
$$\underline{B}=\frac{1}{c}\underline{\hat{R}}\times \underline{E}.$$
$$\underline{v}=\frac{dw(t)}{dt};\;\underline{a}=\frac{d\underline{v}}{dt};\;\underline{u}=c\underline{\hat{R}}-\underline{v}.$$
The Lorentz force over charged particle $Q$ is 
$$F=\frac{qQ}{4\pi\varepsilon_{0}} \frac{R}{(\underline{R}\cdot \underline{u})^2}\left[ [(c^2-v^2)\underline{u}+\underline{R}\times(\underline{u}\times \underline{a})]+\frac{v}{c}[\underline{R}\times[(c^2-v^2)\underline{u}+\underline{R}(\underline{u}\times \underline{a})]] \right].$$
The Poynting vector is given by
$$\underline{S}=\frac{1}{c\mu_{0}}(\underline{E}\times(\underline{\hat{R}}\times \underline{E}))=\frac{1}{\mu_{0}c}[E^2\underline{\hat{R}}-(\underline{\hat{R}}\cdot \underline{E})\underline{E}]$$
Considering the radiation field term in the $\underline{E}$ field:
$$E_{rad}=\frac{q}{4\pi\varepsilon_{0}} \frac{R}{(\underline{R}\cdot \underline{u})^3}(\underline{R}\times(\underline{u}\times \underline{a}))=\frac{q}{4\pi\varepsilon_{0}} \frac{R}{(\underline{R}\cdot \underline{u})^3}(\underline{u}(\underline{R}\cdot \underline{a})-\underline{a}(\underline{R}\cdot \underline{u})).$$
$E_{rad}$ is perpendicular to $\underline{R}$ so $\underline{\hat{R}}\cdot \underline{E}=0$ so
$$S=\frac{1}{c\mu_{0}}E_{rad}^2\underline{\hat{R}}.$$
In the particles rest frame, $\underline{u}=c\underline{\hat{R}}$:
$$\underline{R}\cdot \underline{E}_{rad}=\frac{q}{4\pi\varepsilon_{0}} \frac{R}{(cR)^3}[c\underline{\hat{R}}(\underline{R}\cdot \underline{a})-c\underline{a}(\underline{R}\cdot \underline{\hat{R}})]$$
$$=\frac{q\mu_{0}}{4\pi R}[\underline{\hat{R}}(\underline{\hat{R}}\cdot \underline{a})-\underline{a}].$$
$$E_{rad}^2=\left( \frac{q\mu_{0}}{4\pi R} \right)[(\underline{R}\cdot \underline{a})^2-2(\underline{R}\cdot \underline{a})+\underline{a}^2]$$
which in the radiation limit gives
$$E_{rad}^2=\left( \frac{q\mu_{0}}{4\pi R} \right)[a^2-(\underline{\hat{R}}\cdot \underline{a})^2\underline{\hat{R}}].$$
Given $\underline{\hat{R}}\cdot \underline{a}=a\cos \theta$, we get a Poynting vector of
$$\underline{S}=\frac{1}{\mu_{0}c}\left( \frac{q\mu_{9}}{4\pi R} \right)a^2\sin^2\theta.$$
This gives the power radiated as
$$P_{rad}=\oint \underline{S}\cdot d\underline{a}=\frac{q^2\mu_{0}a^2}{6\pi c}.$$
This is Larmor's formula - valid in the particle's rest frame.