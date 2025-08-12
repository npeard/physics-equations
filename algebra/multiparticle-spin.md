# Calculating Total Spin of Multiparticle States

The total spin squared operator for a single particle is:
$$\hat{S}^2 \ket{sm} = \hbar^2 s (s+1) \ket{sm}$$

For two spin-1/2 particles, the total spin operator becomes:
$$\hat{S}^2 = (\hat{S}_1+\hat{S}_2)^2 = \hat{S}_1^2 + \hat{S}_2^2 + 2 \hat{S}_1 \cdot \hat{S}_2 = \hat{S}_1^2 + \hat{S}_2^2 + 2 (\hat{S}_1)_z (\hat{S}_2)_z$$

For the aligned state:
$$\hat{S}^2 \ket{\uparrow \uparrow} = \hbar^2 \left( \frac{1}{2}\left(\frac{1}{2}+1\right)+\frac{1}{2}\left(\frac{1}{2}+1\right)+2\frac{1}{2}\frac{1}{2}\right) \ket{\uparrow \uparrow} = 2\hbar^2 \ket{\uparrow \uparrow}$$

This implies that $s(s+1) =2$ so the total spin $s=1$ for this state.

For the symmetric Bell state:
$$\hat{S}^2 \frac{1}{\sqrt{2}} (\ket{\uparrow \downarrow} + \ket{\downarrow \uparrow}) = \frac{2 \hbar^2}{\sqrt{2}} (\ket{\uparrow \downarrow} + \ket{\downarrow \uparrow})$$

This also gives total spin $s=1$, making it a triplet state and a maximally entangled Bell state.

The antisymmetric Bell state $\frac{1}{\sqrt{2}} (\ket{\uparrow \downarrow} - \ket{\downarrow \uparrow})$ is a singlet state with total spin $s=0$.
It is also a Bell state.