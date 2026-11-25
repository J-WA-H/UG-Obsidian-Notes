Consider the [structure function](Structure%20Functions.md) of a nucleon
$$F(X)=X\sum_{c}Q_{c}^2f_{c}(X)$$
where $f_{c}(X)$ is the individual PDF and $Q_{c}$ is the charge.
For example, a [proton](Proton%20Structure.md) has
$$F(X)=X\sum_{q}\sum_{t=s,v}Q_{c}^2(C(x)+\bar{C}(X))$$
where $q(X)$ is the structure function for valence and the normal sea quarks, and $\bar{q}(X)$ is the for sea anti quarks, as there are no valance sea quarks. This sums over $q$, the quark type, and $t$, which is either the valence or sea quarks.

For electron-proton scattering, where there are valence quarks $uud$ and sea quarks $u\bar{u},d\bar{d},c\bar{c},s\bar{s},t\bar{t},b\bar{b}$:
$$F^p(X)=X\left[ \frac{1}{9}(d^{p}_{v}(X)+d^{p}_{s}(X)+\bar{d}^{p}_{s}(X))+\frac{4}{9}(u^p_{v}(X)+u^{p}_{s}(X)+\bar{u}^{p}_{s}(X))+\frac{1}{9}(s^{p}_{s}+\bar{s}^p_{s})+c+b+t \right].$$
In the proton there are a lot of up, down quarks, some some strange quarks, very few charm quarks and essentially no top/bottom quarks.

For the Neutron, we can write the same
$$F^N(X)=X\left[\frac{1}{9}(d^{N}_{v}(X)+d^{N}_{s}(X)+\bar{d}^{N}_{s}(X))+\frac{4}{9}(u^N_{v}(X)+u^{N}_{s}(X)+\bar{u}^{N}_{s}(X))+s+c+b+t\right].$$
The proton has valence quarks $uud$ and the neutron has valence quarks $udd$. 
PDFs give how many particles there are for a given $X$, and quarks show the same properties independent of what hadron they are in.
This means that the structure function for an up quark in a proton is the same for a down quark in a neutron.
$$u_{v}^p=d_{v}^N;\;d_{v}^p=u_{v}^N$$
For valence quarks the structure functions are the same independent of whether they are in a proton or neutron.
$$q_{s}^p=q_{s}^N=\bar{q}_{s}^p=\bar{q}_{s}^N.$$
This means we can write the neutron PDF in terms of the proton PDF,
$$F^N(X)=X\left[ \frac{1}{9}(u_{v}^p+u_{s}^p+\bar{u}_{s}^p)+\frac{4}{9}(d_{v}^p+d_{s}^p+\bar{d}_{s}^p)+s+c+t+b \right].$$
The down contribution to $F^N$ is given by the up contribution to $F^p$, and the up contribution to $F^N$ is given by the down contribution to $F^p$.

