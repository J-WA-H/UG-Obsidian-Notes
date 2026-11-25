The 4-velocity, $\vec{v}=v^a\vec{e}_{a}$ is determined by the curvature of the path if no physics is happening.
$$\frac{d\vec{v}}{d\tau}=0\tag{6.1} ,$$or the [absolute derivative](Parallel%20Transport.md) of the components
$$\frac{Dv^a}{d\tau}=0=\frac{dv^\alpha}{d\tau}+ \Gamma^\alpha_{\;\beta \gamma} \frac{dx^\beta}{d\tau} \frac{dx^\gamma}{d\tau}= \frac{d}{d\tau}\left( \frac{dx^\alpha}{d\tau} \right)+\Gamma^\alpha_{\;\beta \gamma} \frac{dx^\beta}{d\tau} \frac{dx^\gamma}{d\tau}=\frac{d^2x^\alpha}{d\tau^2}+\Gamma^\alpha_{\;\beta \gamma} \frac{dx^\beta}{d\tau} \frac{dx^\gamma}{d\tau}\tag{6.2}, $$where $\tau$ is the proper time.
Using Newton's derivative notation,
$$\ddot{x}^\alpha+\Gamma^\alpha_{\;\beta \gamma}\dot{x}^\beta \dot{x}^\gamma=0\tag{6.3}. $$
Suppose $s=a\tau$, this is an affine parameter, which can also be used as a geodesic. These are any parameters linear in proper time. This specific one is the path length.
$$\ddot{x}^a+\Gamma^a_{\;bc}\dot{x}^b\dot{x}^c=0\tag{6.4} $$where the dot is now the derivative with respect to any affine parameter.

In 3D cartesian flat space,
$$ds^2=dx^2+dy^2+dz^2,\;g_{ij}=\mathrm{diag}(1,1,1)\tag{6.5}. $$
The [[Christoffel Symbols]] are all zero so the geodesic equations become
$$\ddot{x}^i=0\tag{6.6} $$which is easy to integrate. Using the affine parameter $s$-path length
$$\frac{dx^j}{ds}=a\implies x^j=as+b\tag{6.9} $$so on a flat cartesian surface, the geodesic path is a straight line at a constant speed. Geodesic paths are inertial frames.

On the surface of a sphere, it is too hard to do this in full generality. Instead, we take a path and see if it is geodesic. Take parameter curves. Suppose we take an azimuthal path,
$$s=a\phi \tag{6.10} ,\;\theta=\theta_{0}=const.$$
The only non-zero Christoffel symbols are
$$\Gamma^\theta_{\;\phi \phi}=-\sin \theta_{0}\cos \theta_{0},\;\Gamma^\phi_{\;\theta \phi}=\Gamma^\phi_{\;\phi \theta}=\cot \theta_{0}\tag{6.11} .$$We now check if $(6.10)$ satisfies the equations
$$\frac{d^2x^A}{ds^2}+\Gamma^A_{\;BC} \frac{dx^B}{ds} \frac{dx^C}{ds}=0\tag{6.12} .$$
Splitting this into its two composite equations gives
$$\frac{d^2\theta}{ds^2}+\Gamma^\theta_{\;BC} \frac{dx^B}{ds} \frac{dx^C}{ds}=0=\Gamma^\theta_{\;\phi \phi} \frac{d\phi}{ds} \frac{d\phi}{ds}=-\frac{{\sin \theta_{0}\cos \theta_{0}}}{a^2}=0\tag{6.13} $$This shows there are only very specific values of $\theta_{0}=0, \frac{\pi}{2}, \pi$ gives a geodesic path. $\theta_{0}=0,\pi$ are at the poles so there is no azimuthal movement so the only natural path is along the equator.

Verify the second equation
$$\frac{d^2\phi}{ds^2}+\Gamma^\phi_{\;BC} \frac{dx^B}{ds} \frac{dx^C}{ds}=\Gamma^\phi_{\;\theta \phi} \frac{d\theta}{ds} \frac{d\phi}{ds}+\Gamma^\phi_{\;\phi \theta} \frac{d\phi}{ds} \frac{d\theta}{ds}=0\tag{6.14} $$as $s$ has no $\theta$ dependent, so the second geodesic equation is always satisfied. The parameter curve in $\phi$ on the surface of a sphere satisfies the geodesic equations iff $\theta_{0}=0, \frac{\pi}{2}, \pi$.

Geodesic paths are natural paths, inertial frames that gives the shortest distance between two points. This means Lagrangian mechanics can be used to find these paths.
$$\delta \int_{a}^b ds=0\tag{6.15} $$gives the shortest path. The Lagrangian
$$L=T-V\tag{6.16} $$is used to find the minimum action path,
$$\delta \int Ldt=0\tag{6.17} .$$
Geodesic paths have no forces so $L=T$.
$$T=\frac{1}{2}\left( \left( \frac{dx}{dt} \right)^2+\left( \frac{dy}{dt} \right)^2+\left( \frac{dz}{dt} \right)^2 \right)=\frac{1}{2}\left( \frac{ds}{dt} \right)^2.\tag{6.18} $$
We then want to minimise
$$\delta \int \left( \frac{ds}{dt} \right)^2dt=0.\tag{6.19} $$From the Euler-Lagrange equations, the minimal path is given by
$$\frac{d}{dt}\left( \frac{\partial L}{\partial \dot{x}^i} \right)-\frac{\partial L}{\partial x^i}=0\tag{6.20}. $$
The solutions must be the same as the Geodesic equations, however the Euler-Lagrange equation does not have the Christoffel symbols.

For a sphere, $(6.12)$ and $(6.20)$ are equivalent, so the Euler-Lagrange equation can be used to infer Christoffel symbols. Using the Lagrangian on a sphere $L=\frac{1}{2}g_{AB}\left( \frac{dx^A}{ds} \right)\left( \frac{dx^B}{ds} \right)=\frac{1}{2}\left( a^2 \left( \frac{d\theta}{ds} \right)^2+a^2\sin^2\theta \left( \frac{d\phi}{ds} \right)^2\right)$, the equation for $\theta$ is
$$\ddot{\theta}-\sin \theta \cos \theta \dot{\phi}^2=0\tag{6.21} $$
and the geodesic equation is
$$\ddot{\theta}+\Gamma^\theta_{\;BC}\dot{x}^B\dot{x}^C=0=\ddot{\theta}+\Gamma^\theta_{\;\theta \theta}\dot{\theta}^2+\Gamma^\theta_{\;\theta \phi}\dot{\theta}\dot{\phi}+\Gamma^\theta_{\;\phi \theta}\dot{\phi}\dot{\theta}+\Gamma^\theta_{\;\phi \phi}\dot{\phi}^2\implies \Gamma^\theta_{\;\theta \theta}=\Gamma^\theta_{\;\theta \phi}\Gamma^\theta_{\;\phi \theta}=0;\;\Gamma^\theta_{\;\phi \phi}=-\sin \theta \cos \theta \tag{6.22} .$$
For $\phi$,
$$\ddot{\phi}+2\cot \theta \dot{\theta}\dot{\phi}=0\tag{6.23} $$
and the geodesic equation
$$\ddot{\phi}+\Gamma^\phi_{\;BC}\dot{x}^B\dot{x}^C=0=\ddot{\phi}+\Gamma^\phi_{\;\theta \theta}\dot{\theta}^2+\Gamma^\phi_{\;\theta \phi}\dot{\theta}\dot{\phi}+\Gamma^\phi_{\;\phi \theta}\dot{\phi}\dot{\theta}+\Gamma^\phi_{\;\phi \phi}\dot{\phi}^2=\ddot{\phi}+2\Gamma^\phi_{\;\theta \phi}\dot{\theta}\dot{\phi}\implies\Gamma^\phi_{\;\theta \phi}=\Gamma^\phi_{\;\phi \theta}=\cot \theta.\tag{6.24} $$
