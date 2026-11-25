In DFT, we aim to find an equation for the density $\rho$. Using Rayleigh-Ritz,
$$\bra{\psi} T+V_{ee}+V\ket{\psi}<\bra{\psi'}T+V_{ee}+V\ket{\psi'}\tag{8.1}    $$
Using $\psi=\psi[\rho]$ and $\psi'=\psi[\rho']$,
$$\bra{\psi[\rho]}T+V_{ee}\ket{\psi[\rho]}+\bra{\psi[\rho]}V\ket{\psi[\rho]}<\bra{\psi[\rho']}T+V_{ee}\ket{\psi[\rho']}+\bra{\psi[\rho']}V\ket{\psi[\rho']}.\tag{8.2}$$
Now quantify
$$F[\rho]=\bra{\psi[\rho]}T+V_{ee}\ket{\psi[\rho]}\tag{8.3}$$
$$\implies F[\rho]+\int d^3r\rho(\vec{r})V(\vec{r})=E_{gs}<F[\rho']+\int d^3r\rho'(\vec{r})V(\vec{r})\tag{8.4} $$
This holds $\forall$ $\rho'$.
This implies that $E_{V}[\rho']\geq E_{V}[\rho]$. This is the [[Hohenberg-Kohn Theorem]] variational principle of DFT.
External potential $V_{ext}$ has the ground state density $\rho_{0}$ with energy $E_{0}$,
$$E_{V_{ext}}[\rho]=F[\rho]+\int d^3r\rho(\vec{r})V_{ext}(\vec{r})\geq E_{0}\tag{8.5} $$$\forall$ $\rho(\vec{r})$ with $\int d^{3}r\rho(\vec{r})=N$, $\rho(\vec{r})\geq{0}$.

To find the Euler-Lagrange equations of this functional for $\rho_{0}$, use Lagrange multiplier $\mu$,
$$E_{V_{ext}}[\rho]-\mu \int d^{3}r\rho(\vec{r})=F[\rho]+\int d^3r\rho(\vec{r})V_{ext}(\vec{r})-\mu \int d^3r\rho(\vec{r})\geq E_{0}-\mu N\tag{8.6} $$
The functional derivative is
$$\left.\frac{\delta E_{V_{ext}}[\rho]}{\delta \rho(\vec{r})}\right|_{\rho_{0}}=0\tag{8.7} $$which gives the basic equation for DFT,
$$\left.\frac{\delta F[\rho]}{\delta \rho(\vec{r})}\right\rvert_{\rho_{0}}+V_{ext}(\vec{r})-\mu=0\tag{8.8}. $$This replaces the Schrodinger equation and gives the ground state density $\rho_{0}$. This scales linearly with the number of electrons $N$.

The Lagrange multiplier $\mu$ has units of energy and is the chemical potential of the system, but for our purposes it is an arbitrary constant, as the potential is defined up to a constant.
