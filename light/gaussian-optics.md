# Gaussian Optics

A good reference is Sidney A. Self, "Focusing of spherical Gaussian beams," Appl.Opt. 22, 658-661 (1983).

## Gaussian Beam Profile
$$I(r) = I_0 \exp\left(\frac{-2r^2}{w(z)^2}\right) = \frac{2P_0}{\pi w(z)^2} \exp\left(\frac{-2r^2}{w(z)^2}\right)$$

## Rayleigh Range
$$z_R = \frac{\pi w_0^2}{\lambda}$$

## Outside of Rayleigh Range
$$w_0 = \frac{\lambda}{\pi \theta}$$

where $\theta$ is the radial divergence (half-angle).

## Beam Radius
$$w(z) = w_0 \sqrt{1+\frac{z^2}{z_R^2}}$$

## Wavefront Radius of Curvature
$$R(z) = z \left( 1+\frac{z^2}{z_R^2} \right)$$

## Beam Radii at Lens
$$w(z) = w'(z')$$

## Wavefront Curvature at Lens
$$\frac{1}{R(z)} + \frac{1}{R'(s')} = \frac{1}{f}$$

## Gaussian Thin-Lens Equation
$$\frac{1}{z+\frac{z_R^2}{z-f}}+\frac{1}{z'} = \frac{1}{f}$$

## Magnification
$$m = \frac{w_0'}{w_0} = \left|\frac{f}{z-f}\right|\frac{1}{\sqrt{1+\left( \frac{z_R}{z-f} \right)^2}}$$

## Choosing Focal Length for Fibers or "Point" sources
$$f = \frac{D/2}{\tan{\theta}} = \frac{\pi D (\text{MFD})}{4\lambda}$$

## Spot Size of Collimated Source
$$\phi = \frac{4 \lambda f}{\pi D}$$

Remember that beam waist refers to the radius, and spot size typically refers to diameter.