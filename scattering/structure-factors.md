# Structure Factors

## Born Approximation
Scattering is weak and amplitude of incident beam is constant through sample volume.
Can use Fourier transform to represent scattered wave.

## Kinematic Approximation
Absorption, refraction, and multiple scattering can be neglected.

## Molecular Structure Factors
For molecules, the atomic form factors are convolved with the arrangement of the nuclei:
$$\psi_s(Q) = \sum_{j=1}^N f_j e^{-i q \cdot r_j}$$

$$I(q) = |\psi_s(Q)|^2 = \sum_{j,k=1}^N f_j f_k^* e^{-i q \cdot (R_j - R_k)}$$

$$S(q) = \frac{1}{\sum_{l=1}^N f_j^2} \sum_{j,k=1}^N f_j f_k^* e^{-i q \cdot (R_j - R_k)}$$

Remember that one can arrive at the same expressions by considering an object composed of a convolution of atomic orbitals with delta functions representing nuclear positions.
The Fourier transform of this expression for the real space object, in the Born approximation, gives the product of the atomic structure factor and the structure dependent term - this is the same structure factor as above.

## Useful Identity
$$\sum_{ij}^\nu e^{i q (x_i-x_j) } = \left|\sum_k^\nu e^{i q x_k} \right|^2$$

Remember that in a real experiment there is a finite exposure time such that the measurement is really a time average over nuclear position, charge fluctuation, etc.

## Lattice Structure Factors
For scattering from a lattice, the scattering from different unit cells interferes constructively and thus we can worry only about the composition of a single unit cell plus how many unit cells are in the crystal.

$$F_{hkl} = \sum_{j=1}^N f_j e^{-2 \pi i (h x_j + k y_j + l z_j)}$$

This is the structure factor for a perfect lattice defined by the Miller indices $(hkl)$ of the reciprocal lattice and the real space positions of the atoms in the unit cell along with the atomic scattering factor.
Note here that since the dimensions of the reciprocal lattice are defined by the wavelength, the Miller indices contain the wavelength dependence of $Q = 2\pi/\lambda$.
There is still Q-dependence of the atomic scattering factor $f_j$.

Plugging in the positions of each type of atom in the unit cell, it is simple to derive a set of conditions for $F_{hkl} = 0$ to determine which reciprocal lattice points have no reflection.
These absences from the diffraction pattern determine the symmetry.
The relative intensity of the reflections determine the atom type.

Reciprocal space is always centrosymmetric (allows inversion, see Friedel's Law) and does not allow translations.
There are only 11 Laue groups and their symmetry is lower than the crystal space group.
For example, space group $(P2_1 / c, P2, C2/c, P4_3 2_1 2)$ is point group $(2/m, 2, 2/m, 422)$ is Laue group $(2/m, 2/m, 2/m, 4/mmm)$.
Point group plus translations equals the space group.
Point symmetries include rotation, rotating inversion (rotation plus inversion? isn't this just a mirror?), and mirrors.
Space symmetries further include screw axes and glides.
Chiral molecules will never be found in space groups with inversion, mirrors, or glides.
The Laue group is the point group plus inversion.