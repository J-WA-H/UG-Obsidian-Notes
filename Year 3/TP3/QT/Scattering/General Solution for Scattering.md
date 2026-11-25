Consider the potential
![[Pasted image 20250124151025.png]]
Suppose the potential has full strength $r\leq d$ and is negligible $r>d$. If we solve to get $R^{-}_{\ell}$ for $r\leq d$, we need to solve
$$\left[ \frac{1}{r^2} \frac{d}{dr}\left( r^2 \frac{d}{dr} \right)+k^2-U(r)-\frac{\ell(\ell+1)}{r^2} \right]R_{\ell}^{-}(r)=0.$$
For $r\geq d$, $U(r)\approx 0$, we get the [free solution](Phase%20Shifts.md) 
$$\therefore R_{\ell}^{+}(r)=A_{\ell}(k)[b_{\ell}(k)j_{\ell}(kr)-c_{\ell}(k)n_{\ell}(kr)]=D_{\ell}[j_{\ell}(kr)-\tan(\delta_{\ell})n_{\ell}(kr)].$$
As the wavefunction must be continuous, $$R_{\ell}^{-}(d)=R_{\ell}^{+}(d)$$$$\frac{dR^{-}_{\ell}}{dr}\left|_{r=d}=\frac{dR_{\ell}^{+}}{dr}\right|_{r=d}.$$
$$\therefore \frac{\frac{dR^{-}_{\ell}}{dr}|_{r=d}}{R_{\ell}^{-}(d)}=\frac{\frac{dR_{\ell}^{+}}{dr}|_{r=d}}{R_{\ell}^{+}(d)}=C(k).$$
As we know $R^{+}_{\ell}(r)$:
$$C(k)=\frac{D_{\ell}(k)[kj_{\ell}'(kd)-k\tan(\delta_{\ell})n_{\ell}'(kd)]}{D_{\ell}(k)[j_{\ell}(kd)-\tan(\delta_{\ell})n_{\ell}(kd)]}$$
$$\implies \tan(\delta_{\ell})=\frac{{C(k)j_{\ell}(kd)-kj'_{\ell}(kd)}}{C(k)n_{\ell}(kd)-kn_{\ell}'(kd)}.$$
For the square well:
![[Pasted image 20250124152541.png]]
s-wave phase shift:
$$k\cot(\delta_{0})=-\frac{1}{a}+\mathcal{O}(k)$$
$$\implies a\approx r_{0}\left( {\frac{1-\tan(\sqrt{ U_{0} }r_{0})}{\sqrt{ U_{0} }r_{0}}} \right).$$
Where $a$ is the scattering length.
If $\sqrt{ U_{0} }r_{0}=\frac{(2n+1)\pi}{2}$ then $a$ will diverge. The cross section will be a maximum which leads to resonance.