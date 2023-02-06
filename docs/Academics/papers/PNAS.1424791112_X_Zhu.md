> ## Classification of charge density waves based on their nature
>><mark style="background: #FFF3A3A6;">Journal Ref. [pnas.1424791112](https://doi.org/10.1073/pnas.1424791112)</mark> 
--- 

### Keywords 
- [[CDW]]
- Strong Coupling
- [[Fermi surface nesting]]

### Idea of the paper 
- Failure of traditional approach to [[CDW]] in real systems.
- Electron-phonon coupling(EPC) determining the characteristic phase of CDW.
- Using the published result on CDW system $2H-NbSe_2$, it is shown that $\vec{q}$-dependent EPC can describe CDW better than [[Fermi surface nesting]].
- Extracting EPC matrix element from electronic band and phonon measurements to identify EPC.
- Large EPC do not induce CDW phase(e.g., $Bi_2Sr_2CaCu_2O_{8+\delta}$)

### Summary 
The origin of [[CDW]] lies in the instability of a 1D system described by [[Peierls Transition]]. The extension of this concept to reduced dimensional systems has led to [[Fermi surface nesting]] which dictates that the wave vector($q_{CDW}$) of the CDW and the corresponding lattice distortion. The idea is that segments of the Fermi contours are connected by $q_{CDW}$, ==resulting in the effective screening of phonons== inducing Kohn anomalies in their dispersion at $q_{CDW}$, driving a lattice restructuring at low temperatures.

The paper discusses the motivation behind the [[Strong coupling approach to CDW]] and briefly describes the[[CDW#Experimental Methods to analyze CDW | Experimental Methods to analyze CDW]]. To illustrate the importance of EPC in the formation of CDW, the widely studied system $NbSe_2$ has been described. A CDW phase transition occurs with $q_{CDW}$ ≅ $(2/3 |\Gamma M| = 0.695 Å^{-1}$ (Γ and M are the points at the center and boundary in the Brillouin zone (BZ), respectively, in the high-temperature phase) at $T_{CDW}$ = 33.5 K.  

![[FS_and_susceptibility_NbSe2.png]]

Fig. A shows the [[Fermi surface]] contours obtained from tight binding fit to [[ARPES]] data and $\vec{q}_{CDW}$ obtained from diffraction measurements. The absence of FSN can be seen in the real and imaginary parts of the susceptibility $\chi_0(\vec{q})$ plotted from the experimental data in the Γ–M direction in Fig. (B) and (C). There is no sign of any structure at the FSN values of $\vec{q}_{CDW}$. 

![[order_param_resistivity_anomaly.png]]

Fig. (F) shows the structural transition order parameter with the critical temperature at $T_{CDW}$ = 33.5 K. Fig.(G) displays the measured resistivity as a function of temperatures, clearly showing the superconducting phase transition at $T_S$ but almost no change at the CDW transition temperature $T_{CDW}$. There is no gap in the electronic system, i.e., no insulating state associated with the low-temperature CDW state, inconsistent with that predicted by the Peierls model. 

## Momentum dependent EPC
The $\vec{q}$-dependent EPC is described by the matrix element ${|g(\vec{k},\vec{k^\prime})|}^2$ that couples electronic states $\vec{k}$ and $\vec{k^\prime}$ with a phonon of wave vector $\vec{q}=\vec{k}-\vec{k^\prime}$ and energy $\hbar \omega$. Making the assumption ${|g(\vec{k},\vec{k^\prime})|}^2 = {|g(\vec{q})|}^2$, 

$\Gamma_{EPC}(\vec{q}) = -2{|g(\vec{q})|}^2 Im[\chi(\omega,\vec{q})]$

Where, $\Gamma_{EPC}(\vec{q})$ is the phonon linewidth. 

==The interacting susceptibility== $Im[\chi(\omega,\vec{q})$ ==carries the information from both electron–phonon and electron–electron interactions.==

!!! note
	Read the paper for more explanation for this part.

Experimentally it is not feasible to obtain the interacting $Im[\chi(\omega,\vec{q})]$ and hence authors used an alternative approach. They used the measured band structure which contains both electron-phonon and electron-electron coupling as the input to calculate the Lindhard response function $Im[\chi_0(\omega =0,\vec{q})] = Im[\chi_0(\vec{q})]$(see Fig.(C))

![[EPC_matrix_element.png]]

The strong Kohn-like anomaly observed in 2H-$NbSe_2$ arises from the $\vec{q}$-dependent EPC matrix element with a peak at $\vec{q}_{CDW}$, not from the conventional FSN in the electronic structure. 

!!! question "What happens in systems with large EPC like cuprates?"

Cuprates display different kind of charge ordering(CO) such as stripe phase, a checkerboard phase, special kind of short-range CO phase and long range CO or [[CDW]]s. There is competition between these phases and poses interesting problems. Several works (see [[PNAS.1424791112_X_Zhu#References | References]]) show that simple [[Fermi surface nesting]] is not the driving force of EPC and also that phonon measurements show strong EPC in the low temperature (below 150K) regime. 

Unlike the case in 2D layered materials like $NbSe_2$, neither FSN nor EPC is directly relevant to the CO or CDW phases in cuprates. A recent STM study demonstrated that the observed modulations of the electronic structure in cuprates are unconventional density waves, where antiferromagnetic and Coulomb interactions may play a key role. In any case, whatever the CO phase in cuprates is, it is not a conventional CDW.

![[Re_Img_from_ARPES_cuprates.png]]

In the Fig.(D) above, we see a peak in $Re[\chi(\vec{q},0)]$ at q ∼ $0.41 Å^{−1}$ and from this we might argue that this system would support a CDW, but there is no peak in $Re[\chi(\vec{q},80 \text{ meV})]$ at this momentum. Fig. (D), Inset, shows $Im[\chi(\vec{q},80 \text{ meV})]$ with a peak at q ∼ $0.18 Å^{−1}$, which is also present in $Re[\chi(\vec{q},80 \text{ meV})]$, indicating that there could be a Kohn-like anomaly in the $A_{1g}$ phonon branch at this q. However, nothing is seen in the phonon dispersion or linewidth at this small q. ==It illustrates that although the shape of the susceptibility function is important for determining the characteristics of== ${|g(\vec{k},\vec{k^\prime})|}^2$, ==it appears to have little predictive power when it comes to predicting the existence of or the characteristic of a CDW.==

## Classification of CDW
**Type I** :
Type I CDWs are quasi-1D systems with their origin in the Peierls instability (FSN). Here the lattice distortion is a secondary effect and results from the electronic disturbance. The best example may be linear chain compounds. 

**Type II** :
Type II CDWs are driven by EPC, but not by FSN. Here the electronic and lattice instabilities are intimately tied to each other, and there is a phonon mode at $q_{CDW}$ going to zero at the transition temperature $T_{CDW}$. There is no reason to have a metal-insulator transition associated with the transition. Type II CDWs have been described in this paper. 

**Type III** :
Type III CDWs are systems where there is a charge modulation (or CO) with no indication of FSN or EPC as the driving force. The best example of type III CDWs may be the cuprates that exhibit CO phenomena. Strong EPC or FSN may exist in those systems, but there is no clear signature that EPC or FSN is essential to the formation of the CDWs.

---

## References
1. [Charge order driven by Fermi-arc instability in Bi2Sr(2-x)La(x)CuO(6+δ)—PubMed](https://pubmed.ncbi.nlm.nih.gov/24356115/)
2. [Inelastic X-ray scattering in YBa<SUB>2</SUB>Cu<SUB>3</SUB>O<SUB>6.6</SUB> reveals giant phonon anomalies and elastic central peak due to charge-density-wave formation—NASA/ADS](https://ui.adsabs.harvard.edu/abs/2014NatPh..10...52L/abstract)



