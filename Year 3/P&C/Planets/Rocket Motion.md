Consider a rocket in a vacuum![[Pasted image 20241024193934.png]]
Conservation of momentum implies
$$mv=(m+dm)(v+dv)+(-dm)(v-v_{e}).$$
Neglecting second order $dmdv$ term gives
$$mdv=-v_{e}dm.$$
This gives an ODE than can be solved to give
$$v-v_{0}=v_{e}\ln\left( \frac{m_{0}}{m} \right)\rightarrow\text{ Rocket Equation}$$
$\Delta v>v_{e}$ when $m_0>em$. Here $e$ is the exponential, not eccentricity.

For a typical rocket, $v_{e}=3.0\text{ km s}^{-1}$, $y=5\implies v_{max}=4.8\text{ km s}^{-1}$, where $y$ is the ratio of wet to dry masses. $y=\frac{m_{0}}{m_{min}}$. The maximum speed is far below Earth's escape velocity so a multi-staged rocket must be used.

First stage of 2 stage rocket:
![[Pasted image 20241025083632.png]]
$m_0=m_1+m_2$ and $x=\frac{m_{2}}{m_{1}}$.
Mass of fuel in the first stage $=m_1-\frac{m_1}{y}$. Hence:
$$v_{1}=v_{e}\ln\left( \frac{m_{0}}{m_{0}-\frac{m_{1}(y-1)}{y}} \right).$$
![[Pasted image 20241025084126.png]]
($m_2$ is moving at $v_2$, not $v_1$.

$$v_{2}=v_{e}\ln\left( \frac{y^2(1+x)}{xy+1} \right).$$
Typically $x\approx 0.1$, $y=5$, $v_e=3\implies v_{2}=8.7\text{ km s}^{-1}$. This is still smaller than Earth's escape velocity so typically a three stage rocket is needed.