From [observations](Dark%20Matter%20From%20Galaxy%20Clusters.md) we know that dark matter has $\Omega_{DM_{0}}=0.25$, it is non-relativistic and it is weakly interacting.
Any theoretical candidate for Dark matter must obey these properties.

Looking at the standard model, the only neutral weakly interacting particles are neutrinos. These have an upper bound on mass of $m_{\nu}=0.13\text{ eV/c}^2$, which is a very small mass.

Today the neutrino temperature is
$$T_{\nu}=\left( \frac{4}{11} \right)^{1/3}T_{CMB}\approx 1.946\text{ K}.$$
From this, $k_{B}T\approx 1.68\times 10^{-4}\text{ eV}\ll m_{\nu}c^2$ so they are non-relativistic.

This satisfies two properties of dark matter - weakly interacting and non-relativistic.

To find the neutrino density parameter, consider the neutrino timeline.
![[Pasted image 20250226151417.png]]
Consider neutrinos thermally produced at $k_{B}T= 1\text{ MeV}$; at this temperature, neutrinos are highly relativistic - this is why this theory is called hot dark matter - they had high energies at their birth.

When neutrinos are highly relativistic, the energy density is
$$\rho_{\nu}c^2=n_{\nu}E_{\nu}.$$
As they are relativistic,
$$\rho_{\nu}c^2=\frac{g_{*,\nu}}{2} \frac{4\sigma T^4}{c}$$where$$g_{*,\nu}=\frac{7}{8}\times{3}\times{2}.$$
The factor of 3 is from the fact there are 3 neutrino flavours and the factor of two takes into account their corresponding antiparticles.

At neutrino decoupling, $k_{B}T\approx 1\text{ MeV}$, neutrinos are still highly relativistic so
$$n_{\nu}^{dec}=\frac{\frac{g_{*,\nu}}{2} \frac{4\sigma T^4}{c}}{3k_{B}T}=\frac{2g_{*,\nu}\sigma T^3}{4k_{B}c}=\frac{7\sigma T_{\nu,dec}^3}{2k_{B}c}.$$
Assume the number density of all 3 flavours are the same,
$$n_{\nu_{e}+\bar{\nu}_{e}}^{dec}=n_{\nu_{\mu}+\bar{\nu}_{\mu}}^{dec}=n_{\nu_{\tau}+\bar{\nu}_{\tau}}^{dec}=\frac{1}{3}n_{\nu}^{dec}=\frac{7\sigma T_{\nu,dec}^3}{6k_{B}c}.$$
After neutrino decoupling, no new neutrinos are produced so $n_{\nu}\propto a^{-3}$
$$n_{\nu}(a)=n_{\nu}^{dec} \left( \frac{a_{dec}}{a} \right)^{3}.$$
$$n_{\nu}(a)=\frac{7\sigma}{2k_{B}c}T_{\nu,dec}^{3}\left( \frac{a_{dec}}{a} \right)^{3}=\frac{7\sigma}{2k_{B}c}\left( T_{\nu,dec} \frac{a_{dec}}{a} \right)^{3}=\frac{7\sigma}{2k_{B}c}T_{\nu}^{3}(a)$$
where $T_{\nu}\propto a^{-1}$.

After neutrinos become non-relativistic,
$$\Omega_{\nu_{0}}=\frac{8\pi G}{3H_{0}^{2}}\rho_{\nu_{0}}=\frac{8\pi G}{3H_{0}^{2}}n_{\nu_{0}}m_{\nu}.$$
More rigorously since there are 3 flavours of quarks,
$$\Omega_{\nu_{0}}=\frac{8\pi G}{3H_{0}^{2}}(n^{0}_{\nu_{e}+\bar{\nu}_{e}}m_{\nu_{e}}+n_{\nu_{\mu}+\bar{\nu}_{\mu}}^{0}m_{\nu_{\mu}}+n_{\nu_{\tau}+\bar{\nu}_{\tau}}^{0}m_{\nu_{\tau}})$$
$$=\frac{8\pi G}{3H_{0}^2} \frac{7\sigma T^3_{\nu_{0}}}{6k_{B}c}(m_{\nu_{e}}+m_{\nu_{\mu}}+m_{\nu_{\tau}})$$
$$=\frac{8\pi G}{3H_{0}^2} \frac{7\sigma T^3_{\nu_{0}}}{6k_{B}c}\sum_{i}m_{i}c^2$$
$$=\sum_{i}m_{\nu_{i}}c^2\left( \frac{H_{0}}{100\text{ km s}^{-1}\text{Mpc}^{-1}} \right)^{-2} \frac{8\pi G}{3(100\text{ km s}^{-1}\text{Mpc}^{-1})} \frac{7}{6} \frac{\sigma T_{\nu_{0}}^{3}}{k_{B}c^3}$$
$$=\frac{\sum_{i}m_{\nu_{i}}c^2}{90\text{ eV}}\left( \frac{H_{0}}{100\text{ km s}^{-1}\text{Mpc}^{-1}} \right)^{-2}\ll 0.25$$
since $m_{\nu_{i}}$ is of order $\text{ eV/c}^2$.

As this is much smaller than the observed dark matter density parameter, neutrinos can't be the full picture.
