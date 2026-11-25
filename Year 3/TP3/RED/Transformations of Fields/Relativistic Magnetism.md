Consider a wire and an observer a distance $S$ away from it.
![[Pasted image 20241126184724.png]]
Moving to the rest frame of the charge $q$, we get
$$v'_{\pm}= \frac{{v\mp u}}{1\mp uv/c^2}$$
where $v_{+}$ is the speed of the positive charges and $v_{-}$ is the speed of the negative charges.
Proof that $\lvert v'_{-} \rvert>\lvert v_{+}' \rvert$:
$$v'_{-}=\frac{{v-u}}{1+uv/c^2};\;v_{+}'=\frac{{v-u}}{1-uv/c^2}.$$
Assume
$$\frac{{v+u}}{1+uv/c^2}> \frac{{v-u}}{1-uv/c^2}\implies(v+u)\left( 1-\frac{uv}{c^2} \right)> (v-u)\left( 1+\frac{uv}{c^2} \right)$$
$$\implies u-\frac{uv^2}{c^2}> \frac{v^2u}{c^2}-u\implies 2u> \frac{v^2}{c^2}u.$$
This holds true as $v^2/c^2>1\;\forall\;v$.

Consider the rest frame of the charges, the charge density in this frame is given by
$$\lambda_{0}=\frac{Q_{0}}{L_{0}}.$$
In the $S'$ frame, $L=\frac{L_{0}}{\gamma}$ so
$$\lambda_{\pm}=\pm \frac{Q_{0}}{L_{\pm}}=\pm \gamma_{\pm} \frac{Q_{0}}{L_{0}}=\pm \gamma_{\pm} \lambda_{0}.$$
In $S$, the charge density is given by $\lambda=\gamma(v)\lambda_{0}$.
In $S'$,
![[Pasted image 20241126190050.png]]
the net charge density is given by $\lambda_{tot}=\lambda_{+}-\lambda_{-}=\lambda_{0}(\gamma_{+}-\gamma_{-})$.
$$\gamma_{+}=\frac{{1-uv/c^2}}{\sqrt{ 1-v^2/c^2 }\sqrt{ 1-u^2/c^2 }}=\frac{{1-uv/c^2}}{\sqrt{ 1-u^2/c^2 }}\gamma(v);$$$$\gamma_{-}=\frac{{1+uv/c^2}}{\sqrt{ 1-v^2/c^2 }\sqrt{ 1-u^2/c^2 }}=\frac{{1+uv/c^2}}{\sqrt{ 1-u^2/c^2 }}\gamma(v).$$
This yields a total charge density of
$$\lambda_{0}=\frac{{\lambda_{0}2uv/c^2}}{\sqrt{ 1-u^2/c^2 }}\gamma(v).$$
The $E$ field in $S'$ is given by
$$E'=\frac{\lambda_{tot}}{2\pi\varepsilon_{0}}S\implies F'=qE'=\frac{\lambda v}{\pi\varepsilon_{0}c^2S} \frac{qu}{\sqrt{ 1-u^2/c^2 }}.$$
From [[4-Force]], the transformations of the force is given by
$$F_{\perp}=\frac{1}{\gamma}F'_{\perp};\;F_{\parallel}=F_{\parallel}'.$$
Since $F'$ is orthogonal to the boost, $F=F'/\gamma(u)=\sqrt{ 1-\frac{u^2}{c^2} }F'$
$$=-\frac{\lambda v}{\pi\varepsilon_{0}c^2} \frac{qu}{S}.$$
We know $F=q(\underline{u}\times \underline{B})$
$$=-qu\left( \frac{\mu_{0}I}{2\pi S} \right)$$
where the $B$ field was found from Biot-Savert's law.