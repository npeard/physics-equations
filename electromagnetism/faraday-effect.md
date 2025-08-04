# Faraday Rotation Theory and Mechanisms

The simplest explanation for the Faraday rotation is that the circular oscillation of electrons or dipole moments in a magnetic field produces different indices of refraction for circularly-polarized light of different handedness. 
Classically, we can observe circular birefringence in a material composed of electric dipole moments as follows. 
Beginning with the Lorentz force law for an electron fixed to an atom in a magnetic field, 
 
$$F_e = -e (\vec{E} + \frac{\vec{v}}{c} \times \vec{B} ) $$

we can write the equation of motion of the electron as 

$$m \frac{d^2 \vec{s}}{dt^2} + m \omega_0^2 \vec{s} = -e (\vec{E} + \frac{1}{c} \frac{d \vec{s}}{dt} \times \vec{B} ) $$

where $\vec{s}$ is the displacement vector of the dipole oscillation restricted to the plane perpendicular to the direction of the $\vec{B}$ field (for simplicity, we will take $\vec{B} = B \hat{z}$) and $\omega_0$ is the natural frequency of oscillation of an individual electron in an atom.

If an electromagnetic wave now stimulates oscillation of the atom at frequency $\omega$, then all quantities have an $e^{-i\omega t} $ time-dependence in equilibrium and the equation of motion reduces to  

$$ (\omega_0^2-\omega^2) s_x - i \omega_c \omega s_y = -\frac{e}{m} E_x $$

$$ (\omega_0^2-\omega^2) s_y - i \omega_c \omega s_x = -\frac{e}{m} E_y $$

where $\omega_c = \frac{eB}{mc}$ is the cyclotron frequency. We can write the electric-field and displacement vectors for circularly-polarized waves as 

$$ E_{\pm} = E_x \pm i E_y  \quad s_{\pm} = s_x \pm i s_y  $$

Inserting these expressions into the planar equation of motion above obtains 

$$ (\omega_0^2 - \omega^2 - \omega_c \omega ) s_+ = -\frac{e}{m} E_+ $$

$$ (\omega_0^2 - \omega^2 + \omega_c \omega) s_- = -\frac{e}{m} E_- $$

The induced dipole moments are then 

$$ P_{\pm} = \frac{n_e e^2 E_{\pm} }{m (\omega_0^2-\omega^2 \mp \omega_c \omega)} $$

where $n_e$ is the number density of electrons. We can then find the polarizability via $\chi_{\pm} = 4 \pi P_{\pm} / E_{\pm} $ and finally see the circular birefringence 

$$ n_{\pm} = \sqrt{1 + \frac{4 \pi n_e e^2}{m(\omega_0^2-\omega^2 \mp \omega_c \omega)}} $$

Clearly, $n_+ > n_-$ so the left-hand wave will travel at a slightly lower phase velocity than the right-hand wave. 
The accumulated phase difference between the co-propagating circular waves amounts to a rotation of the linear polarization, hence the name Faraday rotation. 
Note that the birefringence is due entirely to the cyclotron frequency term. 
If the magnetic field were zero, we would have $n_+ = n_-$ and no birefringence. 
The dependence of the Faraday rotation on the presence of a magnetic field leads to this effect being classified as a magneto-optical property of materials. 

We can calculate the amount of rotation of the linear polarization as follows. Based on our calculation of the refractive index, we can write the electric field vector of the circularly-polarized waves as 
```math
\vec{E}_+ = \frac{E_0}{\sqrt{2}} \begin{pmatrix} \cos(\frac{\omega n_+ z}{c} - \omega t) \\\ i \sin(\frac{\omega n_+ z}{c} - \omega t) \\\ \end{pmatrix} 
```
```math
\vec{E}_- = \frac{E_0}{\sqrt{2}} \begin{pmatrix} \cos(\frac{\omega n_- z}{c} - \omega t) \\\ i \sin(\frac{\omega n_- z}{c} - \omega t) \\\ \end{pmatrix} 
```
from which we can write the vector for the combined linearly-polarized wave 

$$ \vec{E} = \frac{E_0}{\sqrt{2}} \begin{pmatrix} \cos(\frac{\omega n z}{c} - \omega t) \cos(\frac{\omega}{2c} [ n_+ - n_-] z) \\\ \cos(\frac{\omega n z}{c} - \omega t) \sin(\frac{\omega}{2c} [ n_+ - n_-] z) \\\ \end{pmatrix} $$

where $n = \frac{1}{2} (n_+ + n_-)$ is the average refractive index. 
The polarization angle is then 

$$ \theta = \arctan \left( \frac{E_y}{E_x} \right) = \frac{\omega}{2c} (n_+ + n_-) z $$

Evidently, we should expect the polarization angle to change linearly with distance propagated through the material.

Given a 1T magnetic field, the cyclotron frequency will be about 30 GHz. 
For our purposes, we are interested in light with a wavelength around 10 microns or a frequency of about 30 THz. 
Given the three orders of magnitude that separate these frequencies we can make the following approximation, 
```math
n_+ - n_- \approx \frac{4 \pi n_e e^2 \omega \omega_c }{ m(\omega_0^2-\omega^2)^2}
```
so the rotation with propagation distance is given by 
```math
\frac{d\theta}{dz} = \frac{2 \pi n_e e^2 \omega^2 \omega_c }{m (\omega_0^2-\omega^2)^2}
```
If the electromagnetic wave has frequency much higher than the natural oscillation frequence of the atoms, $\omega >> \omega_0$, the change in polarization angle can be written 
```math
\Delta \theta = \frac{e^3 \lambda^2}{2 \pi m^2 c^4} \int_{C} n_e(z) B_{\parallel}(z) dz 
```
but $n_e(z)$ and $B_{\parallel}(z)$ can typically be assumed to be uniform. 

Given prior knowledge of any of the magnetic field, electron density, or source polarization, a measurement of the final polarization angle at different wavelengths can be useful to infer the other unknown properties of the material. 
Astronomers make use of this fact, and use polarimetric measurements of light from distant sources to infer the properties of interstellar media such as gas clouds. 

We derived the Faraday effect by considering a material composed of electric dipoles, but the polarization rotation may also be computed from a model where the material is composed of magnetic dipoles. 
It turns out that the results are identical and both derivations end up with expressions that depend on the refractive index which is a function of both the electric permittivity and magnetic permeability.