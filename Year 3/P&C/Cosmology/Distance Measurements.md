To measure [Hubble's constant](Hubble%20Flow.md), we need the recessional velocity, from [[Redshift]], and the distance, which is normally complicated.

The method to measure distance depends on the cosmic distance ladder,
![[Pasted image 20250204111320.png]]

For nearby stars, parallax is used to measure distance. Measuring the position of a star six months apart shoes the star has moved by an angle $\alpha$, in arcsecs.
![[Pasted image 20250204111519.png]]

The distance to the star in parsecs is
$$d=\frac{1}{\alpha}.$$
For further stars, standard candles are used. A candle is an object with a known luminosity so measuring the flux, $f$, can give the distance
$$f=\frac{L}{4\pi r^2}.$$
As luminosity is not an observable quantity, it must be given by an observable, $X$.
This works for main sequence stars, where $L$ is a function of temperature, $L(T)$, cepheid variable stars, where luminosity is a function of period $L(P)$, and spiral galaxies where it is a function of rotational velocity through the Tully-Fisher relation, $L(V_{rot})$.
The distance is given by
$$r=\sqrt{ \frac{L(X)}{4\pi f} }.$$
To work out $L(X)$, we use closer objects, where we know the distance so we can measure $X$ and $F$ and $r$ so we can calibrate $L(X)$ which can then be used for further objects.

For main sequence stars, the Hertzsprung-Russell diagram can be used to calibrate $L(T)$ by measuring $T,f$ and calculating $L$ using distance $r$ measured using parallax.

For cepheids, this same method can be used but period $P$ is measured instead of temperature, and $r$ can be measured using parallax or main sequence stars.

For nearby galaxies, we can use cepheids in them to measure the distance to them by measuring their period, and flux.

For more distant galaxies, the Tully-Fisher relation or supernovae are used.

The Tully-Fisher relation gives 
$$L\propto V_{rot}^4.$$
A universal strong correlation between the galaxy's luminosity and rotation velocity can be calibrated by measuring $V_{rot},f$ and calculating $L$ using the distance $r$ using cepheids.

For further galaxies, they may be too faint to observe so we need to measure bright objects like supernovae. 

The supernova light curve can be used as a standard candle, which described the brightness over time.
![[Pasted image 20250204114021.png]]

A universal value of supernova's luminosity $L$ regardless of where or when it is can be calibrated by measuring $f$ and calculating $L$ using the distance $r$ measured using cepheids.

Using these distance measurements plotted with recessional velocity gives the Hubble relation, where today the value of Hubble's constant is given to be $H_{0}=72\pm 8\text{ km s}^{-1}\text{Mpc}^{-1}$.

If considering a distant galaxy, with a large galaxy cluster in between, gravitational lensing will occur and the observer will see many images of the galaxy.
![[Pasted image 20250204114858.png]]

The geometric time delay is caused by the difference in the lengths of light paths.

The shift can be calibrated by measuring the time delay in the light curve of two images of the same quasar.
