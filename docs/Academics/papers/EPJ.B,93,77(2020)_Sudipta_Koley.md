> ## Charge density wave and superconductivity in transition metal dichalcogenides
>><mark style="background: #FFF3A3A6;">Journal Ref.  Eur. Phys. J. B (2020) 93: 77</mark> 

---
### Keywords 
- Charge density waves([[CDW]])
- [[Superconductivity]]
- Transition metal dichalcogenides
-  Bogoliubov-de Gennes Theory ([[BdG]])
- [[DFT]]
- [[DMFT]]
- Disorder

### Idea of the paper 
An alternative explanation from [[Strong coupling approach to CDW]] is argued to explain the competition between [[Superconductivity]] and [[CDW]].

By using real-space self-consistent Bogoliubov-de Gennes calculations and momentum-space calculations involving density-functional theory and dynamical mean-field theory, it is shown that there is a surprising reappearance of superconductivity in the presence of non-magnetic disorder fluctuations. 

### Summary 
[[Superconductivity]] and [[CDW]] are considered weak coupling [[Fermi surface]] instabilities mediated by phonons. These orders compete for the same [[Fermi surface]] and when disorder suppresses one, the other one grows at its expense. The original idea of [[CDW]] due to [[Fermi surface nesting]] ([[Peierls Transition]]) do not appear in real system where nesting is scarce. An alternative view is from strong coupling.

Large spectral weight transfer and absence of phonon signatures at typical energies in [[ARPES]] data, along with momentum-independent self-energy, are strong pointers to physics beyond(mean-field) single particle processes. 

**In order to understand the competition, the problem of co-existing [[CDW]] and SC is taken, and a non-magnetic disorder is added to it. Two kinds of disorders are studied: random disorder and clusters of disordered regions of fixed strengths. Using [[BdG]] formulation, the evolution of SC and [[CDW]] is observed by Monte Carlo method. A [[DFT]] followed by multi-orbital [[DMFT]] calculations has been done.** 

#### Results from self-consistent BdG calculations 
- Emergence of superconducting islands increases with increasing disorder even though the disorder is completely uncorrelated from site to site. 
- These superconducting islands are separated from one another by very small CDW regions and the size of the islands is the measure of coherence length and can be tuned with disorder strength and superconducting pair potential.

![[comparison_CDW_SC_disorder.png]]
*variation of $\Delta_{CDW}$ and $\Delta_{SC}$ with disorder strength in (a) clustered disorder configuration, and (b) random disorder configuration.*

- $\Delta_{CDW}$ decreases with disorder strength, while the SC order increases, indicating that emergence of SC order takes place in a highly disordered situation. 
- For longer CDW wavelength, SC is not suppressed much (or by negligible amount) by CDW in the absence of disorder, because the density modulation due to CDW takes place over a length scale which does not affect SC. 
- If CDW has a small wave vector (i.e., rapidly changing carrier density) SC is strongly affected.
- Suppression of the superconductivity by the CDW order decreases with increasing CDW period (or decreasing the values of $Q_x$ and $Q_y$).
- The reentrance of superconductivity in the presence of nonmagnetic potential fluctuation, extracted in analysis of a square lattice, is expected to be present in a triangular lattice also. 

#### Results from DFT+DMFT 
##### DFT
![[bandstructure_TaSe2_TaSeS.png]]
*Band structure of 2H-TaSe2 and 2H-TaSeS*

![[FS_TaSe2_TaSes.png]]
*[[Fermi surface]] 2H-TaSe2 and 2H-TaSeS*

- The band diagram of 2H-TaSe2 shows strong $Ta-d_{z^2}$ character hybridized with Se-p in the two metallic bands crossing the [[Fermi level]] due to two layers of TaSe2 coupled by van der Waals interaction. 
- Similar features are observed for the doped TaSe2.
- Six hole pockets are observed in the [[Fermi surface]] for both the structure. 

##### DMFT
- The parent compound 2H-TaSe2 has two CDW transitions (120 K and 90 K) down to low temperatures and the reported superconductivity is below 1 K($\sim 0.14 K$)
- Examination of CDW state through resistivity in this dichalcogenide shows a change in slope of resistivity around 120 K in 2H-TaSe2, which is the onset of incommensurate CDW.

 ![[DMFT_CDW_TaSe2_TaSeS.png]]
*DMFT resistivity with temperature for x=0 and x=1*

- The resistivity decreases monotonically thereafter without any feature. 
- The onset of commensurate CDW order at 90 K does not reflect in the resistivity, as the condensation of pre-formed excitons already began at a higher temperature.
- Below 5 K, the resistivity suddenly drops sharply to a very small value, indicating the onset of an SC transition at 5 K in the x = 1 alloy. 

##### Strong coupling route 
- An effective model for the incoherent metal is written down and a mean field analysis for the CDW instability is performed thereon. 
- The partial restoration of coherence in the low temperature phase is achieved through excitonic condensation. 
- The resistivity above the instabilities, tellingly, reflects this excitonic fluctuation with a linear behavior at high temperature until CDW or SC order sets in. 
- Disorder brings in a new length scale in the problem and degrades CDW order by localizing charges and suppressing excitonic fluctuations.
- Superconductivity is not affected by disorder, unless it is too strong. *This is primarily the reason why SC shows up at the expense of CDW as disorder increases.* This also implies that the *resistivity actually goes down with disorder initially (till disorder-induced charge localization comes into effect)* in the CDW state, seen in DMFT calculations. 

---

