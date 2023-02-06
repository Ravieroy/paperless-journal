## $AV_3Sb_5$ ARPES
---
## ARPES study for KV3Sb5
Ref.  [Three-dimensional energy gap and origin of charge-density wave in kagome superconductor KV3Sb5 | Communications Materials](https://www.nature.com/articles/s43246-022-00255-1)

!!! abstract
	Kagome lattices offer a fertile ground to explore exotic quantum phenomena associated with electron correlation and band topology. The recent discovery of superconductivity coexisting with charge-density wave (CDW) in the kagome metals $KV_3Sb_5$, $RbV_3Sb_5$, and $CsV_3Sb_5$ suggests an intriguing entanglement of electronic order and superconductivity. However, the microscopic origin of CDW, a key to understanding the superconducting mechanism and its possible topological nature, remains elusive. Here, we report angle-resolved photoemission spectroscopy of $KV_3Sb_5$ and demonstrate a substantial reconstruction of Fermi surface in the CDW state that accompanies the formation of small three-dimensional pockets. The CDW gap exhibits a periodicity of undistorted Brillouin zone along the out-of-plane wave vector, signifying a dominant role of the in-plane inter-saddle-point scattering to the mechanism of CDW. The characteristics of experimental band dispersion can be captured by first-principles calculations with the inverse star-of-David structural distortion. The present result indicates a direct link between the low-energy excitations and CDW, and puts constraints on the microscopic theory of superconductivity in alkali-metal kagome lattices.

### Fermi surface
![[KV3Sb5_ARPES_EXP.png]]
*Figure 1*

- Fig. 1c shows the ARPES-intensity mapping at $E_F$ as a function of $k_x$ and $k_y$ at T = 120 K (above $T_{CDW}$) measured with 114 eV photons which probe the $k_z$ ~ 0 plane of the bulk Brillouin zone
- A circular pocket centered at the Γ point and two (small and large) triangular shaped intensity patterns centered at each K point are resolved, as also visualized in Fig. 1d. 

![[KV3Sb5_ARPES_BANDS.png]]
*Figure 2*

- According to the band structure calculations (Fig. 2), they are attributed to the $5p_z$ band of Sb atoms embedded in the kagome lattice plane (Sb1) and the kagome lattice band with mainly the 3d character of V atoms respectively (note that the small and large triangular features have the dominant $d_{x^2-y^2}$ and $d_{xz/yz}$ character, respectively).
-  The large triangular feature with the V-$3d_{xz/yz}$ character connects to each other around the M point and forms a large hexagonal FS centered at the Γ point.
- The bright spots around the M point originate from the large [[Density of states]] associated with the saddle-point van Hove singularity in the band dispersion.

### Influence of CDW on FS
#### Normal ARPES
- ARPES intensity mappings at T = 20 K and 120 K (Fig. 1c, e) share several common features such as the Γ-centered electron pocket and the triangular pattern around the K point, a closer look reveals some intrinsic differences between them. For example, the intensity around the M point associated with the saddle point is substantially suppressed at T = 20 K due to the CDW-gap opening. 
- The intensity of triangular pockets is strongly distorted at T = 20 K to show a discontinuous behavior at particular k points (black arrows), in contrast to that at T = 120 K which shows a smooth intensity distribution.
- This indicates the reconstruction of FS due to the strong modulation of band dispersion by the periodic lattice distortion associated with the [[CDW]].


| T = 120K > ($T_{CDW}$)          | T = 20K (<$T_{CDW}$) |
| ------------------------------- | -------------------- |
| ![[ARPES_KV3Sb5_T_gr_TCDW.png]] | ![[ARPES_KV3Sb5_T_ls_TCDW.png]]                     |

#### Band dispersion across $T_{CDW}$
| T =20K(<$T_{CDW}$)                | Band dispersion |
| ------------------------------- | --------------- |
| ![[ARPES_KV3Sb5_T_ls_TCDW.png]] | ![[Band_dispersion_T_CDW.png]]                |

Figure (h, i) shows a comparison of the ARPES intensity along a k cut indicated by a red dashed line in Fig. (e) which traverses the reconstructed [[Fermi surface]] at T = 20 K. One can recognize an obvious difference in the intensity distribution between T = 120 K and 20 K in Fig. (h, i). A new holelike band which crosses $E_F$ (indicated by blue circles and lines) appears at T = 20 K in the k region where FS is absent at T = 120 K.

#### Second derivative ARPES 
- Plot of [[ARPES#Second derivative ARPES | second-derivative ARPES]] intensity at T = 20 K in Fig. 1f signifies that the discontinuous intensity distribution (Fig. below) is accompanied by the emergence of a small pocket-like feature near the K point (white dotted ellipse). This pocket is associated with the CDW because it is absent at T = 120 K (Fig. 1d). 

| T = 120K > ($T_{CDW}$)          | T = 20K (<$T_{CDW}$)            |
| ------------------------------- | ------------------------------- |
| ![[ARPES_SD_KV3Sb5_T_gr_TCDW.png]] | ![[ARPES_SD_KV3Sb5_T_ls_TCDW.png]] |
|                                 |                                 |

---

Ref. [Electronic nature of charge density wave and electron-phonon coupling in kagome superconductor KV3Sb5 | Nature Communications](https://www.nature.com/articles/s41467-021-27946-6)

!!! abstract
	The Kagome superconductors $AV_3Sb_5$ (A = K, Rb, Cs) have received enormous attention due to their nontrivial topological electronic structure, anomalous physical properties and superconductivity. Unconventional charge density wave (CDW) has been detected in AV3Sb5. High-precision electronic structure determination is essential to understand its origin. Here we unveil electronic nature of the CDW phase in our high-resolution angle-resolved photoemission measurements on $KV_3Sb_5$. We have observed CDW-induced Fermi surface reconstruction and the associated band folding. The CDW-induced band splitting and the associated gap opening have been revealed at the boundary of the pristine and reconstructed Brillouin zones. The Fermi surface- and momentum-dependent CDW gap is measured and the strongly anisotropic CDW gap is observed for all the V-derived Fermi surface. In particular, we have observed signatures of the electron-phonon coupling in $KV_3Sb_5$. These results provide key insights in understanding the nature of the CDW state and its interplay with superconductivity in AV3Sb5 superconductors.

### Fermi Surface

![[FS_reconstruction_Luo.png]]
The CDW-related 2 × 2 lattice reconstruction generates electronic structure reconstruction.

| ARPES : FS                | Reconstructed FS              |
| ------------------------- | ----------------------------- |
| ![[Luo_KV3Sb5_ARPES.png]] | ![[FS_reconstructed_Luo.png]] |
|                           |                               |

Four [[Fermi surface]](FS) sheets can be seen in the figure (left). FS topology is mainly composed of circular electron like pocket around $\bar{\Gamma}(\alpha)$. A large hexagon-shaped hole-like sheet centered around $\bar{\Gamma}(\beta)$, a triangular hole-like pocket around $\bar{K}(\gamma)$ and a triangular electron-like pocket around $\bar{K}(\delta)$. 

Figure (right) shows the effect of the 2 × 2 lattice reconstruction on the Fermi surface as induced by one of the three wavevectors, $Q_1$. The reconstructed FS is produced by shifting the original lines by the wave vector $\pm Q_1$. Under the measurement geometry used, the observed folded bands are mainly from $\pm Q_1$, while those from $\pm Q_2$ and $\pm Q_3$ are rather weak. ==The electronic reconstruction is also directly evidenced in the measured band structure(see original paper fig. 2c), in which the band measured along  
the $\Gamma - M$ direction coincides with the direction of Q1 wave vector.==

### Signatures of Electron-Phonon coupling

The [[CDW]] state was first proposed for a one-dimensional chain of atoms with an equal spacing a which is argued to be inherently unstable against the dimerized ground state. It usually involves one band with a half electron filling. This would open a CDW gap at the Fermi point $k_F$ = ±π/2a and produce a lattice reconstruction with a wavevector of π/a. Such a [[Fermi surface nesting]] picture is extended to real materials with higher dimensions, where the CDW state is realized because segments of the Fermi surface are nearly parallel, connected by a wavevector $Q_{CDW}$.

The CDW transition typically involves electronic structure reconstruction and lattice distortion, in which the electron–phonon coupling plays an important role. The evidence of this [[Strong coupling approach to CDW]] has been observed in $KV_3Sb_5$. 

| Bandstructure(BS)   | Zoomed BS  &  Self-Energy                 |
| ------------------- | --------------------------- |
| ![[BS_EPC_Luo.png]] | ![[EPC_BS_self_energy.png]]

A kink in the dispersion can be observed in the above figure. The quantitative dispersion is obtained by fitting momentum distribution curves at different binding energies. Taking a linear line as an empirical bare band, the effective real part of the electron self-energy is shown in Fig. (h). It shows a peak at ~36 meV. The observed kink in the energy dispersion and the peak-dip-hump structure in EDCs (see paper) are reminiscent of those from the electron–boson coupling in simple metal and high-temperature superconductors. The phonon frequency of the vanadium vibrations in AV3Sb5 can reach up to ~36meV, that is consistent with the mode energy observed. Therefore, significant self energy effects in $KV_3Sb_5$ is observed. It can be interpreted in terms of electron–phonon coupling, which is present for all bands.

## ARPES study for CsV3Sb5
Ref. [Phys. Rev. Lett. 125, 247002 (2020) – CsV3Sb5: A Z2 Topological Kagome Metal with a Superconducting Ground State](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.125.247002)

- Data collected with differing photon energies did not reveal any appreciable dispersion along $k_z$, consistent with a quasi-2D band structure.
- ARPES data, collected at 50, 80, 100, and 120 K, showed no resolvable change in the band structure when transitioning through the $T^*$ transition. 

![[CsV3Sb5_ARPES_EXP_Ortiz.png]]

---

Ref. [Twofold van Hove singularity and origin of charge order in topological kagome superconductor CsV3Sb5 | Nature Physics](https://www.nature.com/articles/s41567-021-01451-5)

![[CsV3Sb5_FS_ARPES_kang.png]]
Fig.2 *a–d, Fermi surface (a) and constant energy contours at E = −0.15 eV (b), −0.30 eV (c) and −0.45 eV (d) as measured with 95 eV photons. The hexagonal surface Brillouin zones are marked with dashed hexagons.*

![[CsV3Sb5_BS_ARPES_kang.png.png]]


- The Fermi surface of $CsV_3Sb_5$ display the characteristic hexagonal symmetry and Brillouin zone expected from the underlying kagome lattice.
- A circular electron pocket is at the Brillouin zone center $\bar{\Gamma}$, labelled as the G band. The orbital projection from DFT reveals that the G band has dominant Sb character (see [[AV3Sb5 band structure#Orbital-projected electronic structure of CsV_3Sb_5]]).


![[CsV3Sb5_Tomographic_ARPES.png]]

*Tomographic sections of the vHS of K2 (a), K1 (b) and K2′ (c) bands. Panels 1–6 correspond to the energy– momentum slices of Fig. 2a at $k_y$ = −0.76, −0.86, −0.96, −1.06, −1.16 and −1.26 Å−1, respectively.*
