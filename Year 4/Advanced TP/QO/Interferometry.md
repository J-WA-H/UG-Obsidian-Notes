Consider the Mach-Zehnder interferometer.
![[Pasted image 20251111113558.png]]
This is composed of two beam spitters, BS1, BS2, two mirrors M1, M2, two detectors D1, D2, and a phase shifter.

The clockwise path goes from BS1 to M2 to BS2 and the anticlockwise path goes from BS1 to M1 to BS2. There is a phase shifter placed between BS1 and M2 on the clockwise path.

Generally, the phase shifter is represented by a unitary operator $e^{ i\theta \hat{N} }$. The single incident photon on a beam spitter transforms as
$$\ket{0}_{0}\ket{1}_{1}\to \frac{1}{\sqrt{ 2 }}(\ket{0} _{2}\ket{1} _{3}+i\ket{1} _{2}\ket{0} _{3})\to \frac{1}{\sqrt{ 2 }}(e^{ i\theta }\ket{0} _{2}\ket{1} _{3}+i\ket{1}_{2}\ket{0} _{3} )\tag{14.1}  $$
where $e^{ i\theta \hat{N} }\ket{1}_{3}=e^{ i\theta }\ket{1}_{3}$.
We can ignore the common phase due to mirrors.

Consider the second beam splitter, the single photon incident states transform as,
$$\begin{matrix}
\ket{0} _{2}\ket{1} _{3}\to \frac{1}{\sqrt{ 2 }}(\ket{0} _{4}\ket{1} _{5}+i\ket{1} _{4}\ket{0} _{5}) \\
\ket{1} _{2}\ket{0} _{3}\to \frac{1}{\sqrt{ 2 }}(i\ket{0}_{4}\ket{1} _{5}+\ket{1} _{4}\ket{0} _{5} )
\end{matrix}\tag{14.2} .$$
These then superpose to fit the [entangled incident state](QM%20of%20Beam%20Splitters.md), with the superposed solution given by
$$\frac{1}{\sqrt{ 2 }}(e^{ i\theta }\ket{0} _{2}\ket{1} _{3}+i\ket{1} _{2}\ket{0} _{3})\to \frac{1}2 [(e^{ i\theta }-1)\ket{0} _{4}\ket{1} _{5}+i(e^{ i\theta }+1)\ket{1} _{4}\ket{0} _{5}].\tag{14.3} $$
The detector D1 (D2) firing corresponds to detecting $\ket{0}_{4}\ket{1}_{5}$ ($\ket{1}_{4}\ket{0}_{5}$). The corresponding probabilities are given by
$$\begin{matrix}
P_{01}=\frac{1}{2}[1-\cos \theta] \\
P_{10}=\frac{1}{2}[1+\cos \theta]
\end{matrix}\tag{14.4} .$$
This shows that the probabilities depend on the phase $\theta$ so there are interference fringes.

Now consider two incident coherent states. Using the Baker-Campbell-Hausforff identity, we can show that
$$e^{ \beta \hat{a}^{\dagger}-\beta ^{*}\hat{a} }\ket{\alpha} =e^{ \beta\alpha ^{*}-\beta ^{*}\alpha }\ket{\alpha+\beta}.\tag{14.5}  $$
Use this together with
$$\ket{\beta}_{0}\ket{\alpha} _{1}=e^{ \beta \hat{a}_{0}^{\dagger}-\beta ^{*}\hat{a}_{0} }e^{ \alpha \hat{a}_{1}^{\dagger}-\alpha \hat{a}_{1} }\ket{0}_{0}\ket{0} _{1}\tag{14.6}   $$to determine the transformation of the two [[Coherent States]] on a beam splitter.

Two incident coherent states transform generally on a beam splitter as
$$\ket{\beta} _{0}\ket{\alpha} _{1}\to e^{( \beta \hat{a}_{2}^{\dagger}-\beta ^{*}\hat{a}_{2})/\sqrt{ 2 } }e^{ (i\beta \hat{a}^{\dagger}_{3}+i\beta ^{*}\hat{a}_{3})/\sqrt{ 2 } }\ket{i\alpha/\sqrt{ 2 }}_{2}\ket{\alpha/\sqrt{ 2 }}_{3}=\ket{(i\alpha+\beta)/\sqrt{ 2 }}_{2}\ket{(\alpha+i\beta)/\sqrt{ 2 }}    _{3}\tag{14.7}. $$
To consider the effect of the phase shifter, decompose the coherent states into number states,
$$e^{ i\theta \hat{N} }\ket{\alpha} =e^{ -|\alpha|^2/2 }\sum_{n=0}^{\infty} \frac{\alpha^{n}}{\sqrt{ n! }}e^{ i\theta n }\ket{n} =\ket{\alpha e^{ i\theta }}.\tag{14.8}  $$
We now have all the tools necessary to analyse Mach-Zehnder interferometry with coherent states:
BS1:
$$\ket{0}_{0}\ket{\alpha} _{1}\to \ket{i\alpha/\sqrt{ 2 }}_{2}\ket{\alpha/\sqrt{ 2 }}  _{3}\tag{14.9}  $$
Phase shifter:
$$\ket{i\alpha/\sqrt{ 2 }}_{2}\ket{\alpha/\sqrt{ 2 }}_{3}\to \ket{i\alpha/\sqrt{ 2 }}_{2}\ket{e^{ i\theta }\alpha/\sqrt{ 2 }}_{3}\tag{14.10}$$
BS2:
$$\ket{i\alpha/\sqrt{ 2 }}_{2}\ket{e^{ i\theta }\alpha/\sqrt{ 2 }}_{3}\to \ket{i(e^{ i\theta }+1)\alpha/2}_{4}\ket{(e^{ i\theta }-1)\alpha/2}\tag{14.11}  .$$
Phase shift measurements are commonly obtained from the difference in measured intensities which is proportional to the difference number operator
$$\hat{N}_{D}=\hat{a}_{5}^{\dagger}\hat{a}_{5}-\hat{a}_{4}^{\dagger}\hat{a}_{4}.\tag{14.12} $$
$$\langle \hat{N}_{D} \rangle =|\alpha|^2\left[ \sin^2 \frac{\theta}{2}-\cos^2 \frac{\theta}{2} \right]=-|\alpha|^2\cos \theta.\tag{14.13} $$
This is essentially a classical like result.

Quantum fluctuations come from the uncertainty of phase measurements from the calculus of error propagation,
$$\Delta \theta=\sqrt{ \langle \hat{N}_{D}^2 \rangle  -\langle \hat{N}_{D} \rangle ^2}\left( \left\lvert  \frac{{\partial \langle \hat{N}_{D} \rangle }}{\partial \theta}  \right\rvert  \right)^{-1}.\tag{14.14} $$
For a coherent state input,
$$\Delta \theta=\frac{1}{|\alpha||\sin \theta|}.\tag{14.15} $$
This is optimised by $\theta=\frac{\pi}{2}, \frac{3\pi}{2}$ and $|\alpha|\to \infty$.

