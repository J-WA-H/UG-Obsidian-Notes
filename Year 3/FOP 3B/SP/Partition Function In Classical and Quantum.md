We know the [[Partition Function]] for a [single particle](Properties%20of%20Degenerate%20States.md) system is given by
$$Z_{1}=V\left( \frac{2\pi m}{\beta h^2} \right)^{3/2}=\frac{V}{\lambda_{D}^3}.$$
For distinguishable particles (classical), an N-particle system has a partition function of $Z_{N}=Z_{1}^{N}$.
For indistinguishable particles (quantum), an N-particle system has a partition function $Z_{N}=\frac{Z_{1}^{N}}{N!}$.

For distinguishable particles $\ln (Z_N)=\ln(Z_{1}^{N})=N(\ln V-3\ln \lambda_{D})$ and for indistinguishable particles $\ln(Z_{N})=\ln\left( \frac{Z_{1}^{N}}{N!} \right)=N\ln(Z_{1})-\ln(N!)\approx N\ln(Z_{1})-(N\ln(N)-N)=N\left( \ln\left( \frac{Z_{1}}{N} \right)+1\right)=N\left( \ln\left( \frac{V}{N} \right)-3\ln \lambda_{D}+1 \right).$
Using these partition functions we an calculate [thermodynamic properties](Link%20Between%20Statistical%20and%20Thermodynamics.md):
$$U=-N \frac{\partial}{\partial \beta}(\ln Z)$$
As only $\lambda_{D}$ depends on $\beta$, $U$ is the same for both classical and quantum particles,
$$U=\frac{3}{2}Nk_{B}T.$$
For free energy
$$F=-k_{B}T\ln Z$$
Distinguishable:
$$F=-Nk_{B}T[\ln V-3\ln \lambda_{D}].$$
Indistinguishable:
$$F=-Nk_{B}T\left[ \ln\left( \frac{V}{N} \right)-3\ln \lambda_{D}+1 \right].$$
For entropy
$$S=\frac{1}{T}(U-F).$$
Distinguishable:
$$S=\frac{1}{T}\left[ \frac{3}{2}Nk_{B}T+Nk_{B}T(\ln V-3\ln \lambda_{D}) \right]$$
$$=\frac{3}{2}Nk_{B}+Nk_{B}[\ln V-3\ln \lambda_{D}].$$
Indistinguishable:
$$S=\frac{1}{T}\left[ \frac{3}{2}k_{B}T+Nk_{B}T\left( \ln\left( \frac{V}{N} \right)-3\ln \lambda_{D}+1 \right) \right]$$
$$=\frac{5}{2}Nk_{B}+Nk_{B}[\ln V-3\ln \lambda_{D}].$$
Consider the case where we double the size of the system $N\to 2N$.
Distinguishable
$$S^{(2N)}=3Nk_{B}+2Nk_{B}\left[ \ln\left({2V} \right)-3\ln \lambda_{D} \right]$$
Indistinguishable:
$$S^{(2N)}=5Nk_{B}T+2Nk_{B}\left[ \ln\left( \frac{2V}{2N} \right)-3\ln \lambda_{D} \right].$$
The change in entropy between these two systems $$\Delta S=S^{(2N)}-2S^{(N)}=\begin{cases}
0 & \text{indistinguishable} \\
2Nk_{B}\ln(2) & \text{distinguishable}
\end{cases},$$
