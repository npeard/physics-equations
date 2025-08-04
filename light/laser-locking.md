# Laser Locking Techniques

## Beat Note Locking

A beat note lock uses a reference laser and the beating of two laser frequencies on a photodiode to lock the second laser to a constant frequency offset with respect to the reference.
The frequency offset needs to be in the RF regime or optically converted to RF to be compatible with the locking electronics.

The signal on the photodiode (using a bias T to remove constant voltage offset) goes as:
$$I \propto |E_1 \cos(\omega_1 t) + E_{\text{ref}} \cos(\omega_{\text{ref}} t) |^2$$

Expanding this expression:
$$I = E_1^2 \cos^2(\omega_1 t) + E_{\text{ref}}^2 \cos^2(\omega_{\text{ref}} t) + 2 E_1 E_{\text{ref}} \cos(\omega_1 t) \cos(\omega_{\text{ref}} t)$$

The cross term becomes:
$$2 E_1 E_{\text{ref}} \cos(\omega_1 t) \cos(\omega_{\text{ref}} t)  = E_1 E_{\text{ref}} \left( \cos[(\Delta \omega + 2\omega_{\text{ref}}) t] + \cos[\Delta \omega t] \right)$$

where $\Delta \omega = \omega_1 - \omega_{\text{ref}}$.

We can use stages of mixing and low pass filtering to get the beat note down to a longer wavelength for the beat note interference.
One stage of mixing the low frequency $\Delta \omega$ component with a VCO followed by a low pass filter gives:
$$\cos(\Delta \omega t) \cos(\omega_{\text{VCO}} t) = \frac{1}{2} \left( \cos[ (\Delta \omega - \omega_{\text{VCO}}) t] + \cos[(\Delta \omega + \omega_{\text{VCO}}) t] \right) \approx \frac{1}{2} \cos[ (\Delta \omega - \omega_{\text{VCO}}) t]$$

Finally, split the signal, insert a delay line in one arm, remix and low pass to get:
$$\cos[ (\Delta \omega - \omega_{\text{VCO}}) t] \cos[ (\Delta \omega - \omega_{\text{VCO}}) t + \phi] = \frac{1}{2} \left( \cos(\phi) + \cos[2(\Delta \omega - \omega_{\text{VCO}} )t + \phi] \right) \approx \cos(\phi)$$

where $\phi = \tau (\Delta \omega - \omega_{\text{VCO}})$ with $\tau$ as the delay time.
$\delta \propto \cos(\phi)$ is maximal when $\Delta \omega = \omega_{\text{VCO}}$.
This voltage signal $\delta$ can be used to feedback current/piezo control to the laser.
With a beat note lock like this, we can control the frequency offset of the laser from the reference using the VCO.

## PDH Locking to a Stable Cavity

[Section to be expanded with PDH locking theory and equations]