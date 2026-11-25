pn-junctions are materials made of joining a [n-Type Semiconductors](n-Type%20Semiconductors.md) and a [p-type semiconductor](p-Type%20Semiconductors.md).
![[Pasted image 20250220111330.png]]
Consider a p-type silicon, it is made into pn-junction by bombarding it with ion donors.
![[Pasted image 20250220111535.png]]
The structure of the n-type section contains electrons and donor ions, and the p-type has holes and acceptor ions.
![[Pasted image 20250220111823.png]]
This implies there is a concentration gradient at the contact plane between the two materials.

This gradient is evened out to equilibrium where electrons move from the n to p type and holes move from the p to n type.
![[Pasted image 20250220112253.png]]
This diffusion builds positive charge in the n-type and negative charge in the p-type, creating an internal electric field.

The region of the built up charge is the space-charge region.

The diffusion profile is shown as
![[Pasted image 20250220112656.png]]
where holes dominate at the far p-side and electrons dominate at the n-side.

To work out the internal $E$-field, consider the 1D Gauss' law.
$$\frac{d\underline{E}}{dx}=\frac{\rho(x)}{\varepsilon_{r}\varepsilon_{0}}.$$
In the space-charge region (SCR) on the n-side,
$$\frac{dE_{n}}{dx}=\frac{eN_{D}}{\varepsilon_{r}\varepsilon_{0}}\implies E_{n}=\int \frac{eN_{D}}{\varepsilon_{r}\varepsilon_{0}}dx=\frac{eN_{D}}{\varepsilon_{r}\varepsilon_{0}}x+C.$$
Define the boundary condition that the SCR on the n-side only reaches to $x=W_{n}$, so $E_{n}(W_{n})=0$.
$$\implies 0=\frac{eN_{D}}{\varepsilon_{r}\varepsilon_{0}}W_{n}+C\implies C=-\frac{eN_{D}W_{n}}{\varepsilon_{r}\varepsilon_{0}}.$$
$$\therefore E_{n}(x)=\frac{eN_{D}}{\varepsilon_{r}\varepsilon_{0}}(x-W_{n}).$$
On the p-side, which only reaches $x=-W_{p}$ so $E_p(-W_{p})=0$.
$$\frac{dE_{p}}{dx}=-\frac{eN_{A}}{\varepsilon_{r}\varepsilon_{0}}\implies E_{p}=-\frac{eN_{A}}{\varepsilon_{r}\varepsilon_{0}}\int dx=-\frac{eN_{A}}{\varepsilon_{r}\varepsilon_{0}}x+C$$
$$E_{p}(-W_{p})=0=\frac{eN_{A}}{\varepsilon_{r}\varepsilon_{0}}W_{p}+C\implies C=-\frac{eN_{A}W_{p}}{\varepsilon_{r}\varepsilon_{0}}$$
$$\therefore E_{p}(x)=\frac{eN_{A}}{\varepsilon_{r}\varepsilon_{0}}(x+W_{p}).$$
![[Pasted image 20250220114028.png]]
The electric field must be continuous so $E_{p}(0)=E_{n}(0)$
$$-\frac{eN_{D}W_{n}}{\varepsilon_{r}\varepsilon_{0}}=-\frac{eN_{A}W_{p}}{\varepsilon_{r}\varepsilon_{0}}\implies N_{D}W_{n}=N_{A}W_{p}.$$
This defines conservation of charge.
