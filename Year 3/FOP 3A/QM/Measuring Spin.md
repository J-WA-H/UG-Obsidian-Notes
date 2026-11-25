Now we have the [time dependent spin state](Spin%20in%20a%20Magnetic%20Field.md), we can track the evolution of the measurement of spin:
$$\bra{\chi(t)}\hat{S}\ket{\chi(t)}=\bra{\chi(t)}\hat{S}_{x}\ket{\chi(t)}\underline{\hat{x}}+\bra{\chi(t)}\hat{S}_{y}\ket{\chi(t)}\underline{\hat{y}}+\bra{\chi(t)}\hat{S}_{z}\ket{\chi(t)}\underline{\hat{z}}$$
$$\bra{\chi(t)}\hat{S}_{x}\ket{\chi(t)}=\frac{\hbar}{2}\begin{bmatrix}
\cos\left( \frac{\alpha}{2} \right)e^{i\omega_{L}t/\hbar} & \sin\left( \frac{\alpha}{2} \right)e^{-i\omega_{L}t/\hbar}
\end{bmatrix}\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}\begin{bmatrix}
\cos\left( \frac{\alpha}{2} \right)e^{-i\omega_{L}t/\hbar} \\
\sin\left( \frac{\alpha}{2} \right)e^{i\omega_{L}t/\hbar}
\end{bmatrix}.$$
$$=\frac{\hbar}{2}\sin(\alpha) \cos(\omega_{L}t)$$
$$\bra{\chi(t)}\hat{S}_{y}\ket{\chi(t)}=\frac{\hbar}{2}\sin(\alpha)\sin(\omega_{L}t)$$
$$\bra{\chi(t)}\hat{S}_{z}\ket{\chi(t)}=\frac{\hbar}{2}\cos(\alpha)$$
$$\therefore\bra{\chi(t)}\hat{S}\ket{\chi(t)}=\frac{\hbar}{2}\sin (\alpha)[\cos(\omega_{L}t)\underline{\hat{x}}+\sin(\omega_{L}t)\underline{\hat{y}}]+\frac{\hbar}{2}\cos (\alpha)\underline{\hat{z}}.$$
This shows that measurement of the spin vector of a spin-1/2 particle in a magnetic field along the z axis is oscillates in the x-y plane, with the z coordinate remaining constant. This is known as the Larmor procession.