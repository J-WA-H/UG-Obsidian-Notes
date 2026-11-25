Maxwell's equations are
$$\underline{\nabla}\cdot \underline{E}=\frac{\rho}{\varepsilon_{0}}$$
$$\underline{\nabla}\cdot \underline{B}=0$$
$$\underline{\nabla}\times \underline{E}=-\frac{\partial \underline{B}}{\partial t}$$
$$\underline{\nabla}\times \underline{B}=\mu_{0}\underline{j}+\mu_{0}\varepsilon_{0} \frac{\partial \underline{E}}{\partial t}.$$
For any vector $\underline{A}$ we know $\underline{\nabla}\cdot(\underline{\nabla}\times \underline{A})=0$, so we can write $\underline{B}$,
$$\underline{B}=\underline{\nabla}\times \underline{A}.$$
Using Maxwell III, 
$$\underline{\nabla}\times \underline{E}=-\frac{\partial}{\partial t}(\underline{\nabla}\times \underline{A})=-\underline{\nabla}\times\left( \frac{\partial \underline{A}}{\partial t} \right)$$
$$\implies \underline{\nabla}\times\left( \underline{E}+\frac{\partial \underline{A}}{\partial t} \right)=\underline{0}.$$
For any scalar $\phi$ we have $\underline{\nabla}\times(\underline{\nabla}\phi)=\underline{0}$
$$\implies \underline{E}+\frac{\partial \underline{A}}{\partial t}=-\underline{\nabla}\phi$$
so we can rewrite $\underline{E}$:
$$\underline{E}=-\underline{\nabla}\phi-\frac{\partial \underline{A}}{\partial t}.$$
This shows we can rewrite $\underline{E}$ and $\underline{B}$ in terms of the potentials $\phi$, $\underline{A}$.
$$-\underline{\nabla}\cdot \underline{E}=-\nabla^2\phi-\frac{\partial}{\partial t}(\underline{\nabla}\cdot \underline{A})=-\frac{\rho}{\varepsilon_{0}}$$
$$\underline{\nabla}\times(\underline{\nabla}\times \underline{A})=\mu_{0}\underline{j}-\mu_{0}\varepsilon_{0}\underline{\nabla}\left( \frac{\partial \phi}{\partial t} \right)-\mu_{0}\varepsilon_{0} \frac{\partial^2 \underline{A}}{\partial t^2}=\underline{\nabla}(\underline{\nabla}\cdot \underline{A})-\nabla^2\underline{A}$$
$$\implies\left( \nabla^2\underline{A}-\mu_{0}\varepsilon_{0} \frac{\partial^2\underline{A}}{\partial t^2} \right)-\underline{\nabla}\left( \underline{\nabla}\cdot \underline{A}+\mu_{0}\varepsilon_{0} \frac{\partial \phi}{\partial t} \right)=-\mu_{0}\underline{j}$$
