Consider the canonical ensemble, where temperature, volume, and the number of particles is kept constant. The average is
$$\bar{A}=\frac{\sum_{j}A_{j}e^{ -\beta\varepsilon_{j} }}{\sum_{j}e^{ -\beta\varepsilon_{j} }}=\frac{\mathrm{Tr}(Ae^{ -\beta H })}{\mathrm{Tr}(e^{ -\beta H })}\tag{15.1}. $$
The grand canonical ensemble keeps temperature, volume, and energy constant. We want to calculate the thermal occupancy of state $\phi_{i}$: $$\langle \hat{n}_{i} \rangle=\langle a_{i}^{\dagger}a_{i} \rangle =\frac{\mathrm{Tr}(e^{ -\beta(\hat{H}-\mu \hat{N}) }a_{i}^{\dagger}a_{i})}{\mathrm{Tr}(e^{ -\beta(\hat{H}-\mu \hat{N}) })}\tag{15.2}. $$From the [commutator relations](Fermion%202nd%20Quantisation.md),
$$a_{i}a_{i}^{\dagger}-\eta a_{i}^{\dagger}a_{i}=1\qquad \text{where}\qquad \eta=\begin{cases}
+1 & \text{Bosons} \\
-1 & \text{Fermions}
\end{cases}\tag{15.3}. $$
$$\mathrm{Tr}(e^{ -\beta(H-\mu N) }a_{i}^{\dagger}a_{i})=\mathrm{Tr}(e^{ -\beta(H-\mu N) }a_{i}^{\dagger}e^{ \beta(H-\mu N) }e^{ -\beta(H-\mu N) }a_{i})=\mathrm{Tr}(e^{ -\beta(H-\mu N)}a_{i}(e^{ -\beta (H-\mu N) }a_{i}^{\dagger}e^{ \beta(H-\mu N) }) )=\sum_{N}\sum_{\phi^{(N)}}\bra{\phi^{(N)}_{j}} \dots \ket{\phi_{j}^{(N)}} \tag{15.4}. $$
Now we need to evaluate $e^{ -\beta(H-\mu N) }a_{i}^{\dagger}e^{ \beta(H-\mu N) }\ket{\Phi^{(N)}}$. We assume we have a non-interacting system, $H\ket{\Phi_{j}^{(N)}}=E_{j}^{(N)}\ket{\Phi_{j}^{(N)}}$.
$$e^{ \beta(\hat{H}-\mu \hat{N}) }\ket{\Phi^{(N)}}=e^{ \beta(E-\mu N) } \ket{\Phi^{(N)}} =e^{ \beta(E-\mu N) }a_{i}^{\dagger}\ket{\Phi^{(N-1)}} \tag{15.5}. $$For fermions,
$$a_{i}^{\dagger}\ket{\Phi^{(N)}} =\begin{cases}
0 & \phi_{i}\in \ket{\Phi^{(N)}}  \\
\ket{\Phi^{(N+1)}}  & \phi_{i} \notin \ket{\Phi^{(N)}} 
\end{cases}\tag{15.6}. $$
Assume we're either dealing with bosons or the second case for fermions,
$$e^{ -\beta(H-\mu N) }a_{i}^{\dagger}e^{ \beta(H-\mu N) }\ket{\Phi^{(N)}} =e^{ \beta(E-\mu N) }e^{ -\beta(E+\varepsilon_{i}-\mu(N+1)) }a_{i}^{\dagger}\ket{\Phi^{(N)}}=e^{ -\beta(\varepsilon_{i}-\mu) }a_{i}^{\dagger}\ket{\Phi^{(N)}}  \tag{15.7}. $$
This is always true.
$$\implies \langle a_{i}^{\dagger}a_{i} \rangle =\frac{\mathrm{Tr}(e^{ -\beta(H-\mu N) }a_{i}^{\dagger}a_{i})}{\mathrm{Tr}(e^{ -\beta(H-\mu N) })}=\frac{e^{ -\beta(\varepsilon_{i}-\mu) }\mathrm{Tr}(e^{ -\beta(H-\mu N) }a_{i}a_{i}^{\dagger})}{\mathrm{Tr}(e^{ -\beta(H-\mu N) })}.\tag{15.8} $$
$$\implies \langle a_{i}^{\dagger}a_{i} \rangle =e^{ -\beta(\varepsilon_{i}-\mu) } \frac{\mathrm{Tr}(e^{ -\beta(H-\mu N) })}{\mathrm{Tr}(e^{ -\beta(H-\mu N) })}+e^{ -\beta(\varepsilon_{i}-\mu) }\eta  \frac{\mathrm{Tr}(e^{ -\beta(H-\mu N) }a_{i}^{\dagger}a_{i})}{\mathrm{Tr}(e^{ -\beta(H-\mu N) })}\implies \langle a_{i}^{\dagger}a_{i} \rangle =e^{ -\beta(\varepsilon_{i}-\mu) }+\eta \langle a_{i}^{\dagger}a_{i} \rangle e^{ -\beta(\varepsilon_{i}-\mu) }\tag{15.9} $$
$$\implies e^{ \beta(\varepsilon_{i}-\mu) }\langle a_{i}^{\dagger}a_{i} \rangle =1+\eta \langle a_{i}^{\dagger}a_{i} \rangle =\langle a_{i}^{\dagger}a_{i} \rangle=\frac{1}{e^{ \beta(\varepsilon_{i}-\mu) }-\eta}\tag{15.10}. $$
