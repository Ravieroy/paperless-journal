# Strong coupling approach to CDW

!!! quote
	This (Peierls) instability came to me as a complete surprise when I was tidying material for my book (1955), and it took me a considerable time to convince myself that the argument was sound. It seemed of only academic significance, however, since there are no strictly one-dimensional systems in nature. I therefore did not think it worth publishing the argument, beyond a brief remark in the book, which did not even mention the logarithmic behavior.
	^^*Peierls RE (1991) More Surprises in Theoretical Physics (Princeton Univ Press, Princeton), p 29.*^^
## Motivation
The traditional approach to explaining [[CDW]] involves the [[Fermi surface nesting]] which originally was formulated for 1D systems where [[Peierls Transition]] created a fundamental instability. The conjecture was that the gain in electronic energy would always overwhelm the cost of restructuring the atoms. The phonon dispersion for a 1D chain showed[[CDW#Kohn Anomaly | Kohn anomaly]] below and equal to the transition temperature $T_{CDW}$. 

The standard practice to[[Peierls Transition#Extending Peierls picture to 2D and 3D | extend the Peierls picture to higher dimensions]] is to calculate the susceptibility ($\chi(\vec{q},\omega)$) for a given electronic configuration and use the zero energy value of the Lindhard response function $\chi_0(\vec{q}) \equiv \chi_0(\vec{q},\omega=0)$ to determine whether the electron response can drive a Peierls phase transition―there should be a peak in the imaginary part of the response function $Im[\chi_0(\vec{q})]$ at the [[Fermi surface nesting]] (FSN) vector $q_{CDW}$ as well as in the real part $Re[\chi_0(\vec{q})]$, because the real part defines the stability of the system. 

 ![[Lindhard_function.png]]

!!! important
	- If CDWs are created by FSN, the Fermi contour must have been distorted to create nesting as represented by $Re[\chi_0(\vec{q})]$. In a seminal paper, Johannes and Mazin demonstrated that the logarithmic divergence of $Re[\chi_0(\vec{q})]$ is not robust against small deviations from perfect nesting. The dotted line in Fig. (D) illustrates what happens for only a 2% deviation in $k_F$ from perfect nesting and Fig. (D), Inset, shows the effect of including a small “Drude relaxation” in the calculation for the susceptibility.
	- If FSN is the origin of the CDW as in the Peierls picture, the real and imaginary parts of the susceptibility calculated using the measured band structure should both show strong peaks at $q_{CDW}$, there should be a Kohn anomaly in all the phonons (except ones not allowed by symmetry) at $q_{CDW}$, and at least one of the modes must go imaginary at low temperature, inducing a lattice distortion and an electronic gap. 

!!! note
	One may argue that both FSN and EPC are forms of electron–lattice interaction, involving excitations of electrons from filled to empty states. However, they should be distinguished because FSN involves elastic scattering, whereas EPC involves inelastic scattering from the lattice.

Density functional theory calculations were performed for a 1D chain of Na atoms, which should be the best representation of a perfect Peierls system. With the atoms clamped there was no sign of an electronic-only density wave, and relaxation of the ion position in the 1D chain failed to produce any distortion, i.e., no Peierls distortion.
However, if the ions were allowed to move in 2D, the lowest energy state was a zigzag chain, but the electronic gap anticipated in the Peierls CDW phase was missing.

!!! question "How do we know if EPC is strong enough to drive the charge ordering?"
	YBCO could be an apt example to answer this question. Recent phonon measurements (See[[Strong coupling approach to CDW#References | References]]) show signatures of strong EPC in the low-temperature (below 150 K) charge-ordering phase of YBCO. However, the role of EPC in YBCO is substantially different from the role in $NbSe_2$ due to two aspects: 
	1. No phonon softening was observed above 150 K ($T_{CDW}$) and
	2. The energy of the soft phonon modes never approaches zero. 
	 Thus, EPC is not strong enough in cuprates to drive the formation of the CO or CDW phase.

## What is EPC mechanism? 

 The strong- coupling approach views the CDW as a condensate out of a pre-formed excitonic liquid of bad metals. The unconventional CDW found in the parent dichalcogenide is a bose-condensate of pre-formed excitons from high temperature. 

---
## References 
1. [Classification of charge density waves based on their nature | PNAS](https://www.pnas.org/doi/10.1073/pnas.1424791112)
2. [[PNAS.1424791112_X_Zhu | Summary of above(PNAS) paper]]
3. [Phys. Rev. B 73, 205102 (2006)—Fermi-surface nesting and the origin of the charge-density wave in NbSe2](https://journals.aps.org/prb/abstract/10.1103/PhysRevB.73.205102)
4. [Inelastic X-ray scattering in YBa<SUB>2</SUB>Cu<SUB>3</SUB>O<SUB>6.6</SUB> reveals giant phonon anomalies and elastic central peak due to charge-density-wave formation—NASA/ADS](https://ui.adsabs.harvard.edu/abs/2014NatPh..10...52L/abstract)



