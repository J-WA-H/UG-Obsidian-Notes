If a particle of a [degenerate state](Counting%20Degenerate%20States.md) has some property $Q_{j}$ then the average over the system is
$$\langle Q\rangle=\frac{1}{N}\sum_{j}n_{j}Q_{j}.$$
Let states have energy $\epsilon_{j}$, degeneracy $g_j$, and $n_{j}=f_{j}g_{j}$ where $f$ is a [distribution function](Maxwell-Boltzmann%20Distribution.md). 
We know
$$f_{j}=\frac{N}{Z}e^{-\beta\epsilon_{j}},\;Z=\sum_{j}g_{j}e^{-\beta\epsilon_{j}}.$$
This gives
$$\langle Q\rangle=\frac{1}{N} \sum_{j}f_{j}g_{j}Q_{j}=\frac{1}{Z}\sum_{j}g_{j}e^{-\beta\epsilon_{j}}Q_{j}=\frac{\sum_{j}g_{j}e^{-\beta\epsilon_{j}}Q_{j}}{\sum_{j}g_{j}e^{-\beta\epsilon_{j}}}.$$
We can go from a discrete to continuous distribution through $\epsilon_{j}\to\epsilon$ and $\sum\to \int$.
$$\langle Q\rangle= \frac{\int g(\epsilon)e^{-\beta\epsilon}Q(\epsilon)d\epsilon}{\int g(\epsilon)e^{-\beta\epsilon}}.$$
We took energy as our variable when deriving this but we could also use $k$, giving
$$\langle Q\rangle=\frac{\int g(k)e^{-\beta\epsilon(k)}Q(\epsilon)d\epsilon}{\int g(k)e^{-\beta\epsilon(k)}d\epsilon}.$$
We can evaluate $Z$
$$Z=\int_{0}^{\infty}g(\epsilon)e^{-\beta\epsilon}d\epsilon=\int_{0}^{\infty}g(k)e^{-\beta\epsilon(k)}dk=\frac{V}{2\pi^2}\int_{0}^{\infty}k^2e^{-\beta \hbar^2k^2/2m}dk$$
$$Z=V\left( \frac{2\pi m}{\beta h^2} \right)^{3/2}$$
We can simplify this to $Z=\frac{V}{\lambda_{D}}$ where $\lambda_{D}$ is the de Broglie thermal wavelength.