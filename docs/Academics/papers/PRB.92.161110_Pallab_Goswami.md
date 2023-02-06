>## Optical activity as a test for dynamic chiral magnetic effect of Weyl semimetals 
>><mark style="background: #FFF3A3A6;">Journal Ref. Phys. Rev. B 92, 161110(R)(2015)</mark> 

---

### Keywords 
- [[WSM with broken P symmetry]]
- [[Chiral Chemical Potential]] 
- [[Dynamic chiral magnetic effect]]

### Idea of the paper 
A general formula for the dynamic chiral magnetic conductivity of the inversion symmetry breaking(ISB) [[Weyl semimetal]] is calculated. Shows that the measurement of the natural optical activity or rotary power provides a direct confirmation of the existence of dynamic [[chiral magnetic effect]] in [[Inversion symmetry breaking]] [[Weyl semimetal]]. (proposes an experimental test)

**The natural optical activity can be used as a test for the existence of the real part of the dynamic chiral magnetic conductivity of inversion-symmetry-breaking WSMs such as TaAs and NbAs.**

### Summary
- The existence of the nontrivial [[Berry curvature]] requires that the spatial inversion ($\mathcal{P}$) and/or the [[Time reversal symmetry]] ($\mathcal{T}$) are broken.
- Experimentally, only recently have been observed a [[Weyl semimetal]] with [[Inversion symmetry breaking]] phase in TaAs and NbAs
- Due to $\mathcal{T}$ symmetry, an [[Inversion symmetry breaking]] [[Weyl semimetal]] can only support an even number of right and left-hand pairs of [[Weyl fermions]], in contrast to WSMs with broken  $\mathcal{T}$.
- In WSM with broken $\mathcal{T}$, a nonzero anomalous Hall effect serves as the characteristic topological magnetoelectric effect (mediated by non-trivial [[Berry curvature]]).
- In the [[Inversion symmetry breaking]] [[Weyl semimetal]] the anomalous Hall effect identically vanishes.
- [[Inversion symmetry breaking]] [[Weyl semimetal]], on the other hand, has the energy difference between the right and the left-handed Weyl fermions, also known as the [[Chiral chemical potential]], can be naturally nonzero. 
- DCME is a topological magnetoelectric effect of [[Inversion symmetry breaking]] [[Weyl semimetal]], and its possible ramifications in these systems are studied. 
- **This paper shows that the [[Dynamic chiral magnetic effect]] current is intimately related to the natural optical activity of an [[Inversion symmetry breaking]] [[Weyl semimetal]], which is also known as [[Optical gyrotropy]].**

The currents due to [[Optical gyrotropy#Equation for gyrotropic current]] and [[Chiral magnetic effect#Equation for chiral magnetic current]] gives us the following relation,
$$\sigma_{ch}(\textbf{q},w) = i\omega \sigma_g(\textbf{q},w)$$
In the presence of a **nonzero gyrotropic conductivity**, the **refractive indices for the left and the right circularly polarized light become different**, which in turn causes a **rotation of the plane of polarization** for the transmitted light, even **in the absence** of a uniform **external magnetic field**. The amount of rotation of the plane of polarization per unit length is known as the rotary power, and the imaginary part of the gyrotropic conductivity governs the size of the rotary power

### Hamiltonian 
[[Tight-binding model]] of an [[WSM with broken P symmetry]].
>Experimental systems such as TaAs and NbAs are body-centered tetragonal systems which possess 12 pairs of right and left-handed Weyl fermions (altogether 24 Weyl points). There exists no simple [[Tight-binding model]] for such materials. 

$$H = \sum_k \psi_k^\dagger[N_{0,k}\sigma_0 + \mathbf{N_k}\cdot\mathbf{\sigma}]\psi_k$$
where the spin-independent hopping term $N_{0,k}$ and the spin-orbit coupling terms $\mathbf{N_k}$are respectively even and odd under spatial inversion.  We only choose NN hopping terms and obtain $\mathbf{N_k} = t_{SO}[sin(k_1a),sin(k_2a),sin(k_3a)]$ and $\mathbf{N_0} = -2t_1[cos(k_1a),cos(k_2a),cos(k_3a)]$ with $t_1 << t_{SO}$

The Weyl excitations occur around the eight high symmetry points can be seen below (For computational implementation, see [[Weyl points ISB]])

![[WSM_ISB.jpg]]

In addition, $\Gamma$ and M points act as the four right-handed Weyl points, while R and X points are the four left-handed Weyl points. In the vicinity of these points, quasiparticles possess linear dispersion and the Berry curvature acquires the characteristic form of a monopole (antimonopole)

The spin-independent hopping term shifts the Weyl points in the energy space, and gives rise to the chiral chemical potential

---
