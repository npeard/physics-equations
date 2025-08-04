# Atomic Form Factors

## Momentum Transfer
$$|Q| = 2 |k_0| \sin(\theta) = \frac{4\pi}{\lambda}\sin(\theta)$$

## General Form Factor
$$f^0(Q) = \int e^{i Q \cdot r} \rho(r,\theta)$$

## Spherically Symmetric Case
For spherical symmetry $\rho(r,\theta) = \rho(r)$, setting $Q \cdot r = |Q||r| \cos(\theta)$:
$$f^0(Q) = 2\pi \int_0^\infty r^2 \rho(r)\,dr \int_0^\pi \sin(\theta) e^{i Qr\cos(\theta)}\,d\theta = 4\pi \int_0^\infty r^2 \rho(r) \frac{\sin(Qr)}{Qr}\,dr$$

## Normalized Form Factor
With $\frac{1}{4\pi}$ normalization for integration over $d\Omega$:
$$f^0(Q) =  \int_0^\infty r^2 |R_{nl}(r)|^2 \frac{\sin(Qr)}{Qr}\,dr$$

for the radial wave functions.

## Single Electron in 1s Orbital
For a single electron in the 1s orbital:
$$f^0_{100}(Q) = \frac{1}{\left( 1+\frac{Q^2 a_0^2}{4Z^2} \right)^2}$$