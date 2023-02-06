# Angle resolved photoemission spectroscopy(ARPES)
---
## Basic Outline 
ARPES is an experimental method based on the photoelectric effect. Electrons in solids can absorb incident photons with energy larger than the work function of the host material, typically a few electronvolts, and escape into the vacuum. These photoemitted electrons, also known as photoelectrons, are collected by an electron analyzer that measures their kinetic energy and momentum. From these measurements, the original band structure is extracted.

The electronic band structures directly visualized by ARPES can provide straightforward evidence of the topological characteristics of topological quantum materials(TQMs). The fact that ARPES is sensitive to both bulk and surface electrons makes it possible to obtain a comprehensive understanding of complex bulk and surface electronic structures, such as topological surface states in topological insulators, Dirac and Weyl fermions in bulk states, and the associated surface Fermi arcs.

As an ARPES measurement under one photon energy probes the band dispersion along a 2D surface in the 3D momentum space, light sources with tunable photon energy (e.g., a synchrotron radiation light source) are needed to obtain the band structure covering the whole 3D BZ. Scanning the photon energy, the probed 2D surface in the momentum space sweeps through the entire 3D BZ; thus, characteristic electronic features of TQMs in the bulk phase, including the Dirac points and Weyl points that reside at certain momenta in the 3D BZ, can be located and observed.

In addition to measuring the electronic states as a function of momentum and energy, I(k, E), thanks to developments in the past couple of decades, ARPES can also explore other degrees of freedom of electrons, including their spin polarization, spatial distribution, and time evolution. Such a complete ARPES measurement \[measuring I(k, E, r, s, t), where r, s, and t represent location, spin, and time, respectively\] gives the most comprehensive understanding of the electronic states in equilibrium as well as their dynamics.

|                                |     |
| ------------------------------ | --- |
| ![[ARPES_Schematic_Basic.png]] | ![[ARPES_Schematic_Basic_2.png]]    |
	_Principle of modern photoemission spectrometer._

| DOS                    | Band Structure    |
| ---------------------- | ----------------- |
| ![[PE_Energetics.png]] | ![[ARPES_BS.png]] |
|                        |                   |
	*Energetics of photoemission process (left) and simulated ARPES data (right) showing band structure of a 2D-free-electron system*

## Schematics and working 
![[ARPES_schematics.png]]
*Photoelectron spectrometers for ARPES. (a) Simplified depiction of lens modes for a modern analyzer. In angle dispersive mode, electrons of the same emission angle (denoted by color) arrive at the same spatial position on the detector plane. In imaging mode, the real-space position of the electrons is mapped onto the detector, independent of emission angle.*

The hemispherical analyzer is highly versatile (compatible with both pulsed and continuous radiation, at energies from eV to keV) and offers high angle and energy  
resolutions with moderate throughput. A schematic of a generic hemispherical analyzer is shown in Fig. (b). It consists of an input lens column, followed by a hemispherical deflector and finally a 2D electron detector. The lens column images the angular distribution of the electrons onto a slit at the entrance of the hemispherical deflector.

The deflector consists of two concentric hemispherical electrodes with different electrostatic potentials, resulting in a radial electric field that causes the electrons to undergo elliptical orbits. Thus, electrons with different KE are dispersed along the radial dimension onto the detector. At the same time, the electron position orthogonal to this axis is determined by its emission angle within the window accepted by the slit. The detector therefore records the 2D photocurrent distribution with respect to ($E_{kin}$, $\theta_y$).  Energy resolutions of the order of 1 meV are routinely obtained. Typical acceptance angles are $\pm$ 15°, with resolutions down to∼0.1°. 

For mapping the angular distribution orthogonal to the slit, conventionally the sample is rotated with respect to an axis parallel to the slit.

## Second derivative ARPES
The second derivative image (SDI) method is widely applied to sharpen dispersive data features in multi-dimensional spectroscopies such as angle resolved photoemission spectroscopy (ARPES). Here, the SDI function is represented in Fourier space, where it has the form of a multi-band pass filter. 

The need for SDI (and related) filters arises when band features are difficult to observe on top of the incoherent background from multiple-scattering events or from other measurement limitations such as when studying a sample domain smaller than the incident photon beam. They are also used to sharpen features and make it easier to trace dispersions by eye.

---
## References 
1. [Photoemission spectroscopy—from early days to recent applications – F. Reinert](https://iopscience.iop.org/article/10.1088/1367-2630/7/1/097/meta)
2. [Visualizing electronic structures of quantum materials by angle-resolved photoemission spectroscopy | Nature Reviews Materials](https://www.nature.com/articles/s41578-018-0047-2)
3. [Rev. Mod. Phys. 93, 025006 (2021) - Angle-resolved photoemission studies of quantum materials](https://journals.aps.org/rmp/abstract/10.1103/RevModPhys.93.025006)





































In ARPES, electron-phonon coupling usually manifests in changing the ‘shape’ of the E vs k (dispersion relation). Without interactions, a bands’ energy evolves smoothly as a function of momentum, but electron-phonon coupling produces ‘kinks’ where the slope is discontinuous (as seen below ~0.07 eV). Further investigation is needed to confirm if a kink originates from electron-phonon coupling or from something else, but the kink is an important clue.

![[e-p_kink.png]]
