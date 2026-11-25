The Von-Neumann equation gives the time evolution of the [[Density Operator]],
$$\rho(t_{0})=\sum_{\alpha=1}^{n}\ket{\alpha(t_{0})} W_{\alpha}\bra{\alpha(t_{0})} .$$
In the Schrodinger picture, at time $t$ the state evolves using the standard evolution operator
$$\ket{\alpha(t)}=U(t,t_{0})\ket{\alpha(t_{0})}  $$
where
$$U(t,t_{0})=\exp\left[ -\frac{i}{\hbar}\hat{H}(t-t_{0}) \right]$$
assuming a time independent Hamiltonian.
$$\rho(t)=\sum_{\alpha=1}^{n}W_{\alpha}\ket{\alpha(t)}\bra{\alpha(t)}  $$
$$=\exp\left[ -\frac{i}{\hbar}\hat{H}(t-t_{0}) \right]\ket{\alpha(t_{0})} W_{\alpha}\bra{\alpha(t_{0})} \exp\left[ \frac{i}{\hbar}\hat{H}(t-t_{0}) \right]$$
$$=U(t,t_{0})\rho(t_{0})U^{\dagger}(t,t_{0}).$$
Take time derivative to give time evolution
$$\frac{d\rho}{dt}=\left[ -\frac{i}{\hbar}\hat{H}\rho(t)+\frac{i}{\hbar}\rho \hat{H} \right]$$
$$\implies i\hbar \frac{d\rho}{dt}=\hat{H}\rho-\rho \hat{H}=[H,\rho(t)].$$
This gives the Von-Neumann equation as the commutator
$$i\hbar \frac{d\rho}{dt}=[H,\rho(t)].$$
This is equivalent to the Liouville equation in classical mechanics which describes the probability in phase space,
$$\frac{d\rho}{dt}=\{ H,\rho \}.$$
The Von-Neumann equation can be used to give the time evolution of the statistical average,
$$\frac{{d\langle A \rangle }}{dt}=\frac{d}{dt}\mathrm{Tr}(\rho A)=\mathrm{Tr}\left( \frac{d\rho}{dt}A \right)=-\frac{i}{\hbar}\mathrm{Tr}([H,\rho]A).$$
$$\therefore \frac{{d\langle A \rangle }}{dt}=-\frac{i}{\hbar}\mathrm{Tr}(H\rho A-\rho HA)=-\frac{i}{\hbar}\mathrm{Tr(AH\rho-HA\rho)}$$
as the trace is cyclical, $\mathrm{Tr}(ABC)=\mathrm{Tr}(CAB)=\mathrm{Tr}(BCA)$.
$$\therefore \frac{{d\langle A \rangle }}{dt}=-\frac{i}{\hbar}\mathrm{Tr}([A,H]\rho).$$
This is the time evolution of the statistical average.
