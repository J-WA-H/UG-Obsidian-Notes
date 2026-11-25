To work out the potential of [[pn-Junctions]], use the definition of the E-field using the [scalar potential](Vector%20and%20Scalar%20Potentials.md) $\phi$,
$$E=-\frac{d\phi}{dx}.$$
On the p-side,
$$E_{p}=-\frac{eN_{A}}{\varepsilon_{r}\varepsilon_{0}}(x+W_{p})=-\frac{d\phi_{p}}{dx}\implies \phi_{p}=\frac{eN_{A}}{\varepsilon_{r}\varepsilon_{0}}\int x+W_{p}dx$$
$$=\frac{eN_{A}}{2\varepsilon_{r}\varepsilon_{0}}(x^2+2W_{p}x)+C$$
Define the boundary condition $\phi(-W_{p})=0$
$$\therefore C=\frac{eN_{A}W_{p}^2}{2\varepsilon_{r}\varepsilon_{0}}\implies \phi_{p}(x)=\frac{eN_{A}}{2\varepsilon_{r}\varepsilon_{0}}(x+W_{p})^2.$$
For the n-side:
$$E_{n}=\frac{eN_{A}}{\varepsilon_{r}\varepsilon_{0}}(x-W_{n})=-\frac{d\phi_{n}}{dx}\implies \phi_{n}=\frac{eN_{A}}{\varepsilon_{r}\varepsilon_{0}} \int x-W_{n}dx$$
$$\phi_{n}=\frac{eN_{D}}{2\varepsilon_{r}\varepsilon_{0}}(x^2-2W_{n}x)+C.$$
Define $\phi_{n}(W_{n})=\phi_{bi}$ so
$$\phi_{n}(x)=\phi_{bi}-\frac{eN_{D}}{2\varepsilon_{r}\varepsilon_{0}}(x-W_{n})^2.$$
![[Pasted image 20250220121946.png]]
![[Pasted image 20250220122416.png]]
Considering the band structure of [[n-Type Semiconductors]] and [[p-Type Semiconductors]], the chemical potential lies at different positions of the band gap. As the two sides are brought together, it goes to equilibrium so the bands follow the shape of the electron energy
![[Pasted image 20250220122905.png]]
Before contact, 
![[Pasted image 20250220154113.png]]
This gives the change in the chemical potential to be
$$e\phi_{bi}=\mu_{n}-\mu_{p};$$
$$\mu_{n}=E_{C}-k_{B}T\ln\left( \frac{N_{C}}{N_{D}} \right);\;\mu_{p}=E_{V}+k_{B}T\ln\left( \frac{N_{V}}{N_{A}} \right).$$
$$e\phi_{bi}=(E_{C}-E_{V})-k_{B}T\ln\left( \frac{N_{C}N_{V}}{N_{A}N_{D}} \right)=E_{g}-k_{B}T\ln\left( \frac{N_{C}N_{V}}{N_{A}N_{D}} \right).$$
Using the law of mass action for [[Intrinsic Semiconductors]],
$$n_{i}^2=N_{C}N_{V}\exp\left[ -\frac{E_{g}}{k_{B}T} \right].$$
$$e\phi_{bi}=\cancel{E_{g}}-k_{B}T\ln\left( \frac{n_{i}^2}{k_{B}T} \right)-\cancel{E_{g}}$$
$$\implies \phi_{bi}=\frac{k_{B}T}{e}\ln\left( \frac{N_{C}N_{V}}{n_{i}^2} \right).$$
To calculate the SCR widths, the fact that $\phi$ must be continuous at $x=0$.
$$\frac{eN_{A}}{2\varepsilon_{r}\varepsilon_{0}}W_{p}^2=\phi_{bi}-\frac{eN_{D}}{2\varepsilon_{r}\varepsilon_{0}}W_{n}^2$$
and using conservation of charge,
$$N_{A}W_{p}=N_{D}W_{A}$$
gives
$$W_{n}=\sqrt{ \frac{2\varepsilon_{r}\varepsilon_{0}}{e}\left( \frac{N_A}{N_{D}} \right)\left( \frac{1}{N_{A}+N_{D}} \right) }$$
$$W_{p}=\sqrt{ \frac{2\varepsilon_{r}\varepsilon_{0}}{e}\left( \frac{N_{D}}{N_{A}} \right)\left( \frac{1}{N_{A}+N_{D}} \right) }.$$