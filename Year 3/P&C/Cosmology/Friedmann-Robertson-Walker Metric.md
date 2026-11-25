Consider a 2D spherical surface of radius $R$.
![[Pasted image 20250121154826.png]]

The infinitesimal change in length across the arc of the 2D surface, $dl$, is given by
$$dl^2=dx^2+dy^2+dz^2.$$
Transfer to spherical coordinates:
$$x=r\cos \theta;\;dx=\cos \theta dr-r\sin \theta d\theta$$
$$y=r\sin \theta;\;dy=\sin \theta dr+r\cos \theta d\theta$$
$$z=\sqrt{ R^2-r^2 };\;dz=\frac{r}{\sqrt{ R-r^2 }}dr.$$
$$\therefore dl^2=\cos^2\theta dr^2+r^2\sin^2\theta d\theta^2-2r\sin \theta \cos \theta d\theta dr+\sin^2\theta dr^2+$$
$$r^2\cos^2\theta d\theta^2-2r\cos \theta \sin \theta drd{\theta}+\frac{r^2dr}{\sqrt{ R-r^2 }}$$
$$=dr^2+r^2d\theta^2+\frac{r^2dr^2}{\sqrt{ R^2-r^2 }}$$
$$=\frac{1}{1-\frac{r^2}{R^2}}dr^2+r^2d\theta^2=\frac{1}{1-kr^2}+r^2d\theta^2$$ where $k=\frac{1}{R^2}$.

For a 3D universe,
$$ds^2=-c^2dt^2+a^2(t)\left[ \frac{dr^2}{1-kr^2}+r^2d\theta^2+r^2\sin ^2\theta d\phi \right].$$
This is the Friedmann-Robertson-Walker metric.

The value of $k$ determines the geometric of the universe:
![[Pasted image 20250121181531.png]]

This metric has a fractional term which is inconvenient, so move $r\to r'$.
![[Pasted image 20250121182424.png]]
As this gets rid of the fraction,
$$dr'=\frac{dr}{\sqrt{ 1-kr^2 }}.$$
$$\implies r'=\int \frac{dr}{\sqrt{ 1-kr^2 }}$$
$$=\begin{cases}
\frac{1}{\sqrt{ k }}\arcsin(\sqrt{ k }r) & k>0 \\
1 & k=0 \\
\frac{1}{\sqrt{ -k }}\text{arcsinh}(\sqrt{ -k }r) & k<0
\end{cases}.$$
This gives the metric
$$ds^2=-c^2dt^2+a^2(t)[dr^2+S_{k}^2(r)(d\theta^2+\sin^2\theta d \phi^2)]$$
where $$S_{k}(r)=\begin{cases}
\frac{1}{\sqrt{ k }}\sin(\sqrt{ k}r) & k>0 \\
r & k=0 \\
\frac{1}{\sqrt{ -k }}\sinh(\sqrt{ -k }r)
\end{cases}.$$
![[Pasted image 20250121183248.png]]
