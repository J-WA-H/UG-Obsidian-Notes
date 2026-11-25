Consider the scattering of two electrons,
![[Pasted image 20260124163054.png]]
The [scattering amplitude](Time%20Evolution.md) is $|S_{fi}|^2\propto |\mathcal{M}^{(a)}+\mathcal{M}^{(b)}|^2$.
Consider
$$|2\mathcal{M}^{(a)}\mathcal{M} ^{(b)}|\propto g_{\mu \nu} \frac{{(\bar{u}_{3}\gamma^\mu u_{1})(\bar{u}_{4}\gamma^\nu u_{2})}}{(p_{1}-p_{3})^2} \frac{{(\bar{u}_{1}\gamma^{\mu'}u_{4})(\bar{u}_{2}\gamma^{\nu'}u_{3})}}{(p_{1}-p_{4})^2}g_{\mu'\nu'}\tag{10.1} $$$$\implies \frac{1}{4}\sum_{pol} \frac{{u_{4}\bar{u}_{4}\gamma^\nu u_{2}\bar{u}_{2}\gamma^{\nu'}u_{3}\bar{u}_{3}\gamma^\mu u_{1}\bar{u}_{1}\gamma^{\mu'}}}{(p_{1}-p_{3})^2(p_{1}-p_{4})^2}g_{\mu \nu}g_{\mu'\nu'}\propto_{m=0}\mathrm{Tr}[p\!\!\!/_{4}\gamma^\nu p\!\!\!/_{2}\gamma^{\nu'}p\!\!\!/_{3}\gamma^\mu p\!\!\!/_{1}\gamma^{\mu'}]g_{\mu \nu}g_{\mu'\nu'}\tag{10.2}. $$To evaluate the trace, we have to consider the properties of the $\gamma$-matrices.
$$\begin{matrix}
\gamma^\mu \gamma_{\mu}=4 \\
\gamma^\mu a\!\!\!/\gamma_{\mu}=\gamma^\mu(\{ a\!\!\!/,\gamma_{\mu}\}-\gamma_{\mu}a\!\!\!/)=2a\!\!\!/-4a\!\!\!/=-2a\!\!\!/ \\
\gamma^\mu a\!\!\!/b\!\!\!/c\!\!\!/\gamma_{\mu}=-2c\!\!\!/b\!\!\!/a\!\!\!/ \\
\gamma^\mu a\!\!\!/b\!\!\!/\gamma_{\mu}=\gamma^\mu a\!\!\!/(\{ b\!\!\!/,\gamma_{\mu} \}-\gamma_{\mu}b\!\!\!/)=2b\!\!\!/a\!\!\!/+2a\!\!\!/b\!\!\!/=2\{ b\!\!\!/,a\!\!\!/ \}=2ab
\end{matrix}\tag{10.3} .$$
Using this and contracting two of the $\gamma$-matrices gives the trace
$$-2\mathrm{Tr}[p\!\!\!/_{4}p\!\!\!/_{3}\gamma^{\nu'}p\!\!\!/_{2}p\!\!\!/_{1}\gamma^{\mu'}]=-8(p_{1}p_{2})\mathrm{Tr}[p\!\!\!/_{4}p\!\!\!/_{3}]=-32(p_{1}p_{2})(p_{3}p_{4}).\tag{10.4} $$
Define Mandelstam variables - consider topologies of $2\to 2$ scattering, $p_{1}p_{2}\to p_{3}p_{4}$.
![[Pasted image 20260124175432.png]]
The propagators spike at $\Delta p^2=m^2$, which causes resonance which is used to detect particles, such as the Higgs boson. The Mandelstam variables are these $\Delta p^2$ values,
$$\begin{matrix}
s=(p_{1}+p_{2})^2=+2p_{1}p_{2} & t=(p_{1}-p_{3})^2=-2p_{1}p_{3} & u=(p_{1}-p_{4})^2=-2p_{1}p_{4}.
\end{matrix}\tag{10.5} $$
Summing these gives $s+t+u=m_{1}^2+m_{2}^2+m_{3}^2+m_{4}^2\to{0}$ as $\forall$ $m\to {0}$.
[[Scattering Amplitudes]] are given by
$$\overline{\sum}|\mathcal{M}^{(t)}|^2\propto \frac{1}{t^2},\;\;\overline{\sum}|\mathcal{M}^{(u)}|^2=\frac{1}{u^2}\;\; \overline{\sum}|\mathcal{M}^{(t)}\mathcal{M}^{(u)}|^2=\frac{1}{tu}\to -\frac{8s^2}{ut}.\tag{10.6} $$
This gives 
$$\overline\sum |M^{(t)}|^2=(u_{3}\bar{u}_{3}\gamma^\mu u_{1}\bar{u}_{1}\gamma^{\mu'})(u_{4}\bar{u}_{4}\gamma^\nu u_{2}\bar{u}_{2}\gamma^{\nu'})g_{\mu \nu}g_{\mu'\nu'}=\mathrm{Tr}[p\!\!\!/_{3}\gamma^\mu p\!\!\!/_{1}\gamma^{\mu'}]\mathrm{Tr}[p\!\!\!/_{4}\gamma^\nu p\!\!\!/_{2}\gamma^{\nu'}]\tag{10.7} $$$$=16[p_{3}^\mu p_{1}^{\mu'}+p_{3}^{\mu'}p_{1}^\mu-g^{\mu \mu'}(p_{1}p_{3})][p_{4}^\nu p_{2}^{\nu'}+p_{4}^{\nu'}p_{2}^\nu-g^{\nu \nu'}(p_{2}p_{4})]g_{\mu \nu}g_{\mu'\nu'}=16[\underbrace{2(p_{3}p_{4})(p_{1}p_{2})}_{s^2/4}+\underbrace{2(p_{3}p_{2})(p_{4}p_{1})}_{u^2/4}]\tag{10.8} $$
$$\implies \overline\sum |\mathcal{M}^{(t)}|^2=\frac{8(s^2+u^2)}{t^2}\tag{10.9}. $$Similarly,
$$\overline{\sum}|\mathcal{M}^{(u)}|^2=\frac{8(s^2+t^2)}{u^2}.\tag{10.10} $$This process for electron-electron scattering can also be used to calculate electron-positron scattering.