Cosmological models can be found by solving the simplified [Friedmann equation](Critical%20Density.md).

Consider a flat-radiation only universe, $\Omega_{R_{0}}=1$, $\Omega_{M_{0}}=\Omega_{\Lambda_{0}}=0$. The Friedmann equation simplifies to
$$\frac{H^2}{H_{0}^2}=\Omega_{R_{0}}a^{-4}$$
$$H^2=H_{0}^2a^{-4}$$
$$H=H_{0}a^{-2}$$
$$\frac{\dot{a}}{a}=H_{0}a^{-2}\implies a\dot{a}=H_{0}$$
$$\implies \int\frac{d}{dt}\left( \frac{1}{2}a^2 \right)dt=\int H_{0}dt$$
$$\frac{1}{2}a^2=H_{0}t+c.$$
Fix $c=0$ as we need $a(0)=0$ for a big bang.
$$a(t)=(2H_{0}t)^{1/2}=\left( \frac{t}{t_{0}} \right)^{1/2};\;t_{0}=\frac{1}{2H_{0}}.$$
$$\implies H(t)=\frac{1}{2t}\implies \ddot{a}<0.$$
For a flat matter universe, $\Omega_{M_{0}}=1,\;\Omega_{R_{0}}=\Omega_{\Lambda_{0}}=0$, the same method can be used to get
$$a(t)=\left( \frac{3}{2}H_{0}t \right)^{2/3}=\left( \frac{t}{t_{0}} \right)^{2/3};\;t_{0}=\frac{2}{3H_{0}}$$
$$\implies H_{0}=\frac{2}{3t}\implies \ddot{a}<0.$$

For a flat $\Lambda$ only universe,
$$a(t)=\exp[H_{0}(t-t_{0})]$$
$$H(t)=H_{0} \implies \ddot{a}> 0.$$
For an empty universe, $\Omega_{R_{0}}=\Omega_{M_{0}}=\Omega_{\Lambda_{0}}=0$:
$$a(t)=H_{0}t=\frac{t}{t_{0}};\;t_{0}=\frac{1}{H_{0}}$$
$$\implies H(t)=\frac{1}{t}\implies \ddot{a}=0.$$
For a non-flat matter universe:
$$H^2=H_{0}a^{-3}[\Omega_{M_{0}}-(\Omega_{M_{0}}-1)a]$$
For $\Omega_{M_{0}}-1>0\implies$ universe is closed, $k>0$.
When
$$a=\frac{\Omega_{M_{0}}}{\Omega_{M_{0}}}-1,\; H=0\implies \dot{a}=0.$$
At some point the universe will reverse its expansion and contract.
For $\Omega_{M_{0}}-1<0\implies$ open universe, $k<0$:
$$\left( \frac{\dot{a}}{a} \right)^2=H^2=H_{0}[\Omega_{M_{0}}a^{-3}-(\Omega_{M_{0}}-1)a^{-2}]$$
$$\dot{a}^2=H_{0}[\Omega_{M_{0}}a^{-1}-(\Omega_{M_{0}}-1)].$$
As $a\to \infty$, the first term goes to zero so $\dot{a}$ is a constant, which moves towards an empty universe.

For a model with matter and $\Lambda$:
$$\frac{H^2}{H_{0}}=[\Omega_{M_{0}}a^{-3}+(1-\Omega_{M_{0}})a^{-2}]+[\Omega_{\Lambda_{0}}-\Omega_{\Lambda}a^{-2}]$$
$$=a^{-3}[\Omega_{\Lambda_{0}}a^3-(\Omega_{M_{0}}+\Omega_{\Lambda_{0}}-1)a+\Omega_{M_{0}}]$$
call the brackets $f(a)$, it is highly dependent on $\Omega_{\Lambda_{0}}$.
![[Pasted image 20250128152353.png]]
For large $\Omega_{\Lambda_{0}}$, there is a point in the past where $H=0$.
