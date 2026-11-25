For [simple poles](Poles%20and%20Zeros.md), $f(z)=\frac{g(z)}{z-z_{0}}$, the [residue](Integrating%20Meromorphic%20Functions.md) can be calculated using
$$\text{Res}[f,z_{0}]=g(z_{0})=\lim_{ z \to z_{0} } (z-z_{0})f(z).$$
For a pole of order $n$, $f(z)=\frac{g(z)}{(z-z_{0})^n}$, the residue is
$$\text{Res}[f,z_{0}]=\frac{1}{(n-1)!}\lim_{ z \to z_{0} } \frac{d^{n-1}}{dz^{n-1}}[(z-z_{0})^nf(z)].$$
If $f(z)=\frac{g(z)}{h(z)}$ where $g$ is [analytic](Complex%20Differentiation.md) and $h$ has a simple zero at $z_0$, $h(z_{0})=0$. then the residue can be calculated using
$$\text{Res}[f,z_{0}]=\frac{g(z_{0})}{h'(z_{0})}.$$
Using this and the residue theorem, we can simplify an integral to just a limit.

Example: Find residue of $f(z)=\frac{1}{z\sin z}$.
This function has a pole of order two at $z=z_{0}$. Take [Laurent series](Laurent%20Series.md):
$$\sin z=z-\frac{z^3}{3!}+\dots$$
$$f(z)=\frac{1}{z^2(1-z^2/3!+\dots)}=\frac{1}{z^2(1+\varepsilon)}.$$
As the series for $\sin z$ converges, we call all terms above 1 as $\varepsilon$ where $\lvert \varepsilon \rvert<1$.
$$f(z)=\frac{1}{z^2}\sum_{n=0}^\infty\left( \frac{z^2}{3!} \right)^n=\frac{1}{z^2}\left( 1+\frac{z^2}{3!}+\dots \right)=\frac{1}{z^2}+\frac{1}{6}+\mathcal{O}(z^2).$$
$\frac{1}{z^2}$ is the principal part and $\frac{1}{6}+\mathcal{O}(z^2)$ is the analytic part. From this we can see that $a_{-1}=0$ so $\text{Res}[f,0]=0$.