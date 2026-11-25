When considering [particle collisions](Making%20Heavy%20Particles.md), the $Z^{0}$ hasn't been considered.

Define the R-ratio as the ratio of the number of quarks to the number of leptons, given by the sum over charges
$$R=\frac{3\sum_{q}q^2_{q}}{\sum_{l}q_{l}^2}.$$
The 3 comes from the fact that quarks have [[Colour Charge]]

Since leptons have charge $\pm1$, $q_{l}^2=1$ so
$$R=3\sum_{q}q_{q}^2$$
where the quark type $q$ goes up to the allowed energy $\sqrt{ S }$.
Plotting R-ratio against $\sqrt{ S }$ gives
![[Pasted image 20250314093115.png]]
where there is a step when a new quark flavour is produced, with the gap being the square of the new charge.

Around $\sqrt{ S }=90\text{ GeV}$, the mass of the $Z^{0}$, there is a large peak that represents $Z^{0}$ resonance. Here there are $\sim 10,000$ more $Z^{0}$ than photons so weak interactions are far more likely.
![[Pasted image 20250314093449.png]]
Unlike for electromagnetic interactions, $Z^{0}$ can couple to neutrinos, so this weak interaction an produce neutrinos.
![[Pasted image 20250314093656.png]]
Neutrinos are very light - the [[Cosmic Microwave Background]] tells us that $m_{\nu_{e}}+m_{\nu_{\mu}}+m_{\nu_{\tau}}\sim 0.12\text{ eV}$.

If there is a 4th generation, then $m_{\nu_{4}}> \frac{90}{2}\text{ GeV}$ which cannot be produced by $Z^{0}$.

Unlike electromagnetic and strong interactions, the weak force can change the flavour of quarks using $W^{\pm}$
It can change any of $u,c,t$ to $d,s,b$, and vis-versa - it changes the charge and hence flavour.
e.g. the weak force can change an up quark to a down, strange, or bottom quark.
![[Pasted image 20250314094214.png]]
This shows that $W^{\pm}$ can change generation, while $\gamma,g,Z^{0}$ cannot.

Analogy: Special relativity.
When doing a [[Lorentz Transforms]],
$$x'=\gamma(x-ut)$$
$$t'=\gamma(t-ux)$$
in natural units.
This can be expressed as a matrix equation,
$$\begin{bmatrix}
x' \\
t'
\end{bmatrix}=\gamma\begin{bmatrix}
1 & -u \\
-u & 1
\end{bmatrix}\begin{bmatrix}
x \\
t
\end{bmatrix}.$$
This transformation links space and time - in our frame space and time are separate/orthogonal, and if we change frames, the are linked so are no longer orthogonal.
![[Pasted image 20250314094608.png]]
This principle can be applied as to how the weak force can change quark flavour.

Let every other quark mediator see the quarks as $(u,c,t)$ and $(d,s,b)$ but let $W^{\pm}$ see something else - $(u',c',t')$ and $(d',s',b')$.

Consider the transformation between $\begin{bmatrix}d \\ s\end{bmatrix}$ and $\begin{bmatrix}d' \\ s'\end{bmatrix}$.
Try [[Rotations]]:
$$\begin{bmatrix}
d' \\
s'
\end{bmatrix}=\begin{bmatrix}
\cos\theta_{c} & \sin\theta_{c} \\
-\sin\theta_{c} & \cos\theta_{c}
\end{bmatrix}\begin{bmatrix}
d \\
s
\end{bmatrix}.$$
$\theta_{c}$ is the Cabibbo angle - $22^{\circ}$.
This normalises the probabilities as $\cos^2\theta_{c}+\sin^2\theta_{c}=1$.
![[Pasted image 20250314101836.png]]
The vertex is the weak coupling constant multiplied by the rotation.
$\mathrm{Pr}(u\to d)=|\cos\theta_{c}|^2$, $\mathrm{Pr}(u\to s)=|\sin\theta_{c}|^2$.

Now consider the transform to the bottom quark again.
$$\begin{bmatrix}
d' \\
s' \\
b'
\end{bmatrix}=\begin{bmatrix}
V_{ud} & V_{us} & V_{ub} \\
V_{cd} & V_{cs} & V_{cb} \\
V_{td} & V_{ts} & V_{tb}
\end{bmatrix}\begin{bmatrix}
d \\
s \\
b
\end{bmatrix}.$$
The matrix is the Cabibbo-Maskawa-Kobayashi (CMK) matrix.
The first row represents $u\to d,s,b$
The second row represents $c\to d,s,b$
The third row represents $t\to d,s,b$.

Examples of decays are
![[Pasted image 20250314102457.png]]
The likelihood of each is given by the CMK matrix, $\mathrm{Pr}=|V|^2\implies \mathrm{Pr}(b\to u)=|V_{bu}|^2$.

Using experimental results we can obtain
$$\frac{|V_{ub}|^2}{|V_{cb}|^2}\approx 0.006.$$
In the CMK matrix, the diagonal terms dominate and the off-diagonal terms are smaller. This means particle decays are more likely to stay within the generation.
