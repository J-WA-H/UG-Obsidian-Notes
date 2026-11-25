##### Elastic scattering:
![[Pasted image 20241029200442.png]]

Consider the elastic scattering case when $m_{1}=m_{2}=m$
$$p_{1}^\mu=\left( \frac{E_{1}}{c}, \underline{p} \right);\;p_{2}^\mu=\left( \frac{E_{2}}{c},-\underline{p} \right).$$
$$q_{1}^\mu=\left( \frac{E_{1}'}{c},\underline{q}_{1} \right);\;q_{2}^\mu=\left( \frac{E_{2}'}{c},\underline{q}_{2} \right)$$
Due to conservation of momentum:
$$p_{1}^\mu+p_{2}^\mu=q_{1}^\mu+q_{2}^\mu$$
Equating these [[4-Vectors]]:
$$\left( \frac{2E}{c},\underline{0} \right)=\left( \frac{{E_{1}'+E_{2}}}{c},\underline{q}_{1}+\underline{q}_{2} \right)$$
$$\implies \underline{q}_{1}=-\underline{q}_{2}\implies E_{1}'=E_{2}'=\sqrt{ (mc^2)^2+p^2c^2 }.$$
##### Inelastic scattering
$$p_{1}^\mu+p_{2}^\mu=p_{3}^\mu+p_{4}^\mu+p_{5}^\mu \text{ particle produced in interaction.}$$
Take scalar product
$$(p_{1}^\mu+p_{2}^\mu)^2=p_{1}^2+p_{2}^2+2p_{1}p_{2}$$
Considering $p_{1}$ is at rest, $p_{1}^\mu=(mc,\underline{0})$, $p_{2}^\mu=(m_{2}c\gamma,m_{2}\gamma \underline{v})$.
$$\therefore p_{1}p_{2}=m_{1}m_{2}c^2\gamma$$
so
$$(p_{1}^\mu+p_{2}^\mu)^2=(m_{1}^2+m_{2}^2)c^2+2m_{1}m_{2}c^2\gamma=Q_{f}^2.$$
This gives
$$\gamma=\frac{{Q_{f}^2-(m_{1}+m_{2})c^2}}{2m_{1}m_{2}c^2}$$
$$Q_{f}=\left( c\sum_{i=3}^n m_{i},\underline{0}\right)$$
so
$$\gamma=\frac{{\left( \sum_{i=3}^nm_{i} \right)^2-m_{1}^2-m_{2}^2}}{2m_{1}m_{2}}.$$
Examples:
$$p^+p^+\rightarrow p^+p^+\pi^0.$$
$$\gamma=\frac{{(2m_{p}+m_{\pi})^2-2m_{p}^2}}{2m_{p}m_{\pi}}=\frac{{2m_{p}^2+m_{\pi}^2+4m_{p}m_{\pi}}}{2m_{p}^2}\approx 1.3$$
for $m_{p}=1000\text{ MeV/c}^2$ and $140\text{ MeV/c}^2$.

Pair creation:
![[Pasted image 20241029210826.png]]
For photons
$$p_{1}^\mu=\left(\frac{hf_{1}}{c}, \frac{hf_{1}}{c}\underline{n} \right)\to p_{1}^\mu p_{1\mu}=0$$
which makes sense since photons are massless particles.
For $e^-/e^+$:
$$p_{2}^\mu=\left( \frac{E_{2}}{c},\underline{p}_{2} \right)$$
$$p_{3}^\mu=\left( \frac{E_{3}}{c},\underline{p}_{3} \right)$$
4-momentum conservation:
$$p_{1}^\mu=p_{2}^\mu+p_{3}^\mu$$
$$\implies(p_{1}^\mu-p_{2}^\mu)^2=p_{3}^\mu p_{3\mu}=m_{e}^2c^2$$
$$p_{1}^2=0;\;p_{2}^2=m_{e}^2c^2$$
$$p_{1}p_{2}=\frac{hf_{1}}{c}\left( \frac{E_{2}}{c}-\underline{p}\cdot \underline{n} \right)=\frac{hf_{!}}{c}\left( \frac{E_{2}}{c}-\lvert p \rvert \cos \theta \right)$$
$$\therefore m_{e}^2c^2-2 \frac{hf_{1}}{c}\left( \frac{E_{2}}{c}-\lvert p \rvert  \cos \theta\right)=m_{e}c^2$$
$$\implies 2 \frac{hf_{1}}{c}\left( \frac{E_{2}}{c}-\lvert p \rvert \cos \theta \right)=0.$$
$E_{2}>c\lvert p \rvert\implies p_{1}p_{2}>0$  $\therefore$ this condition can be satisfied.