## Introduction

???+ note
	SC and CDW are symmetry breaking phases characterized by an energy gap in the single-particle spectrum and with order parameters representing the condensation of electron-electron or electron-hole pairs, respectively. 
 
 It is a periodic modulation of charge density, and an accompanying distortion of the crystal lattice ([[Peierls Transition]]). ***When a CDW forms, gaps open at the [[Fermi surface]] at those portions that satisfy the nesting condition.***
 
![[CDW.png]]

*Highly anisotropic band structure* leads to a novel type of ground state called charge-density wave. The condensate is pinned to the underlying lattice by impurities and by boundary effects. This is a collective transport phenomena of electron-hole pairs. 

One dimensional metal coupled to underlying lattice is not stable at low temperatures. The ground state of the coupled state of the coupled electron-phonon system is characterized by a gap in single -particle excitation spectrum and by a collective mode formed by electron-hole pairs involving the wave vector $q=2k_F$. The charge density associated with the collective mode is, 

$$
\begin{equation}
\rho(r) = \rho_0 + \rho_1 \cos(2k_F \cdot r + \phi) 
\end{equation}
$$

Where $\rho_0$ is the unperturbed electron density of the metal, and the condensate is called a Charge density wave.

Similar to superconductors, the order parameter is complex and the phase $\phi$ of the condensate is very important. It's time and spatial derivative is related to the electric current and to the condensate density.  *In the absence of pinning and damping, the condensate can carry current leading to [[Superconductivity]]*. The thermodynamics of CDW state closely resembles that of Superconducting ground state. The gap $\Delta$ in terms of the dimensionless e-p coupling constant is given by,

$$
\begin{equation}
\Delta = 2D \exp(-1/\lambda) 
\end{equation}
$$

 Where D is the one-dimensional bandwidth.

 The collective mode is formed by e-h pairs, involving the wave-vector $2k_F$ as electron and holes on the opposite side of the [[Fermi surface]] are combined to lead to the CDW and to the accompanying lattice distortion. 
 
 The transition temperature $T_p$ is larger than superconducting transition temperature because of large cutoff frequency D appearing in the gap equation (compared to phonon frequency appearing in the superconducting gap).  The mean-field(MF) description neglects the important role of 1D fluctuations, thus leading to finite transition temperature $T_{MF}$ even for strictly 1D metal. Fluctuations strongly suppress the transitions. 
 
- **General Picture :** ***The materials that are composed of chains and are metal at high temperatures show strong 1D correlations along the chain direction even above three-dimensional transition $T_{3D}$, leading to a wide fluctuating region for transition, $T_{3D} < T_p < T_{MF}$.*** Below $T_{3D}$, the correlations on the neighboring chains couple together, leading to 3D long range order. The CDW under such circumstances develops along the chain direction. 

In other words, When we generalize to higher dimensions, the basic idea is that CDWs can be favored in systems with [[Fermi surface nesting]] because the electronic system looks quasi-1D along the direction where nesting occurs. 

![[CDW_distortion.png]]
*CDW or Peierls Distortion*

### Kohn Anomaly

![[Kohn_anomaly.png]]

The zero energy electronic excitations at $2k_F$ effectively screen any lattice motion with this wave vector. The figure above shows the phonon dispersion for 1D chain at different temperatures. Below $T_{CDW}$ the phonon energy at $q = 2k_F$ becomes imaginary, meaning there is a new lattice structure. Above $T_{CDW}$ there is a sharp dip (Kohn anomaly) in the phonon dispersion but no static restructuring.

## Experimental Methods to analyze CDW
1. [[ARPES]] can determine the band structure and the Fermi contour that are needed to calculate the electronic susceptibility. 
2. Electron, X-ray, neutron diffraction can determine the structure, $\vec{q}_{CDW}$ and $T_{CDW}$.
3. Scanning tunneling microscopy ([[STM]]) and spectroscopy can determine the wavelength of the charge modulation as well as the electronic transition temperature. 
4. Inelastic neutron and X-ray scattering can probe the temperature dependence of the Kohn anomaly in the phonon dispersion.
5. Transport measurements can reveal the transition temperature and the metal insulator transition predicted by the Peierls model. 
6. High-resolution ARPES data are needed to estimate the strength of the EPC in a CDW system. (phonon dispersion and linewidth measurements are very crucial to understand the origin of CDWs.)

--- 
## Useful Links 
1. [[PNAS.1424791112_X_Zhu |Classification of charge density waves based on their nature]]
2. [[PNAS.1424791112_X_Zhu#Classification of CDW |Classification of CDW]]
3. [[Strong coupling approach to CDW]]

