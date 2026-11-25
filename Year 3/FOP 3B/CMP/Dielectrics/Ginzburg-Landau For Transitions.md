For a uniform solid with zero electric field, close to the [critical temperature](Paraelectric%20Transition.md), the free energy is
$$G_{FE}(T)=G_{PE}+\frac{1}{2}g_{2}(T)P^2+\frac{1}{4}g_{4}(T)P^4.$$
Note that even powers in $P$ as we want $G$ to be independent of the direction of $P$.

Analyse the leading coefficient: $\frac{1}{4}g_{4}(T)P^4$.
This is quadratic in $P^2$ so there are two possible graphs,
![[Pasted image 20250306145048.png]]
As we want a stable minimum, the second graph does not give this so the first graph must be the reality $\therefore g_{4}(T)>0$.

At equilibrium,
$$\frac{dG_{FE}}{dP}=0=P[g_{2}(T)+g_{4}(T)P^2].$$This gives two solutions,
$$P=0$$
for the paraelectric phase and
$$P_{s}=\sqrt{ -\frac{g_{2}(T)}{g_{4}(T)} }$$
for the ferromagnetic phase.

At $T>T_{c}$ (paraelectric) we need an unphysical value of $P_{s}\implies g_{2}(T)>0$.
At $T<T_{c}$ (ferroelectric) we need a physical value of $P_{s}\implies g_{2}(T)<0$.

Expand $g_{4}(T)$ as a Taylor series:
$$g_{4}(T)=g_{4}$$
which is a constant, and for $g_{2}$,
$$g_{2}=\gamma(T-T_{0});\;T_{0}=T_{c};\;\gamma>0.$$
$$\implies P_{s}=\sqrt{ \frac{\gamma(T_{0}-T)}{g_{4}} }.$$
![[Pasted image 20250306145810.png]]
For $T>T_{c}$:
![[Pasted image 20250306145925.png]]
After the external field is applied, there is a small [[Polarisation]] as not all [dipoles](Electric%20Dipole.md) align.

The difference in free energy for the ferroelectric and paraelectric transition is
$$G_{FE}-G_{PE}=\frac{1}{2}g_{2}P^2+\frac{1}{4}g_{4}P^4-EP$$
where the last term is the product of the electric field and the polarisation, taking account for the energy density $\varepsilon=-\underline{P}\cdot \underline{E}$.

At equilibrium,
$$\frac{dG_{FE}}{dP}=0=g_{2}P+\cancelto{0}{g_{4}P}-E$$
$$\therefore \frac{P}{E}=\frac{1}{g_{2}}=\frac{1}{\gamma(T-T_{0})}.$$
Looking at the electric displacement field, 
$$D=\varepsilon_{0}E+P=\varepsilon_{0}\varepsilon_{r}E.$$
$$\therefore \frac{1}{\gamma(T-T_{0})}=\varepsilon_{0}(\varepsilon_{r}-1)\implies\varepsilon_{r}=1+\frac{1}{\varepsilon_{0}\gamma(T-T_{0})}.$$
Using [[Ginzburg-Landau Theory]] for first order transitions,
- Assume a uniform solid, $\underline{E}=\underline{0}$
- Close to the Curie temperature, $G_{PE}(T)=G_{PE}+\frac{1}{2}g_{2}(T)P^2+\frac{1}{4}g_{4}(T)P^4+\frac{1}{6}g_{6}(T)P^6$.
$$g_{6}(T)=g_{6}>0$$
$$g_{4}(T)=-|g_{4}|<0$$
$$g_{2}(T)=\gamma(T-T_{0}).$$
At equilibrium,
$$\frac{dG_{FE}}{dP}=P[g_{2}+g_{4}P^2+g_{6}P^4]=0$$
So for paraelectric,
$$P=0$$
and for ferroelectrics,
$$P^2=\frac{{-g_{4}\pm \sqrt{ g_{4}^2-4g_{6}g_{2} }}}{2g_{6}}.$$
The minimum of this is ferroelectric.
![[Pasted image 20250306151341.png]]
