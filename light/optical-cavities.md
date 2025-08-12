# Optical Cavities

A good reference is Siegman Lasers.

## Finesse
$$\mathcal{F} = \frac{\text{FSR}}{\text{FWHM}} \approx \frac{\pi (R_1 R_2)^{1/4}}{1-\sqrt{R_1 R_2}}$$

where $R_i$ is the mirror reflectivity.

## Mode Frequencies
$$\omega_{qnm} = \left( \frac{2 \pi qc}{2L} + (n+m+1) \frac{c}{L} \arccos{ \pm \sqrt{g_1 g_2}} \right)$$

where $g_i = 1-L/R_i$ and $R_i$ is the mirror radius of curvature.

## Rayleigh Range
$$z_R^2 = \frac{g_1 g_2 (1-g_1 g_2)}{(g_1 + g_2 - 2 g_1 g_2)^2} L^2$$

## Mirror Locations Relative to Beam Waist
$$z_1 =\frac{ g_2 (1-g_1 )}{(g_1 + g_2 - 2 g_1 g_2)} L$$

$$z_2 =\frac{ g_1 (1-g_2 )}{(g_1 + g_2 - 2 g_1 g_2)} L$$

## Waist Spot Size
$$w_0^2 = \frac{L \lambda}{\pi} \sqrt{\frac{g_1 g_2 (1-g_1 g_2)}{(g_1 + g_2 - 2 g_1 g_2)^2}}$$

## Mirror Spot Sizes
$$w_1^2 = \frac{L \lambda}{\pi} \sqrt{\frac{ g_2 }{g_1 (1-g_1 g_2)}}$$

$$w_2^2 = \frac{L \lambda}{\pi} \sqrt{\frac{ g_1 }{g_2 (1-g_1 g_2)}}$$