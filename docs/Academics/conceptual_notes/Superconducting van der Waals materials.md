1. Gapped trivial superconductors : 
	- They are inherently a conventional superconductors. 
	- Examples - NbSe2,
2. Nodal superconductivity and  spin-triplet superconductivity 
	- They are not SC by themselves. 
	- Example - Twisted graphene multilayers 
	- Very low DOS near fermi level. 
	- Not enough electrons. 
	- Can be unconventional SC
	- M.F can even enhance SC (spin-triplet SC) : **Reenterant SC**
3. Gapped topological superconductors 
	- Example - CrBr3/NbSe2

Electronic interactions are responsible for symmetry breaking. 
1. Broken time-reversal symmetry : Classical magnets ($M \rightarrow -M$)
2. Broken crystal symmetry : CDW ($r \rightarrow r + R$)
3. Broken gauge symmetry : Superconductors ($<c_\uparrow c_\downarrow> \rightarrow e^{i\phi}<c_\uparrow c_\downarrow>$)

$$H = \sum_{i,j} t_{ij}c_i^\dagger c_j + \sum_{ijkl} V_{ijkl} c_i^\dagger c_j c_K^\dagger c_l$$
What are these interactions coming from?
- Electronic (repulsive) interactions
- Mediated by other quasiparticles(phonons, magnons, plasmons)
- **The net effective interaction can be attractive or repulsive. SC requires attractive interactions**

With a mean field description : Approximate quadratic Hamiltonian and Effective single particle description. Weakly correlated matter.
$$H \approx \sum_{i,j}\bar{t}_{ij}c_i^\dagger c_j + \sum_{ij} \Delta_{ij} c_i c_j$$


## Origin of attractive interactions 
### Conventional superconductors 
- Phonons
### Unconventional superconductors 
- Antiferromagnetic magnons 
- Ferromagnetic magnons 
- Plasmons 
- Valence fluctuations 
- Charge fluctuations

## A simple interacting Hamiltonian 
$$H = \sum_{ij} t_{ij}[c_{i\uparrow}^\dagger c_{j\uparrow} + c_{i\downarrow}^\dagger c_{j\downarrow}] + \sum_i U c_{i\uparrow}^\dagger c_{i\uparrow} c_{i\downarrow}^\dagger c_{i\downarrow}$$
$U < 0 \rightarrow 0$ : Superconductivity 
Mean field approximation 
$$U c_{i\uparrow}^\dagger c_{i\uparrow} c_{i\downarrow}^\dagger c_{i\downarrow} \approx U <c_{i\uparrow}^\dagger c_{i\downarrow}^\dagger> c_{i\uparrow} c_{i\downarrow} + h.c$$

$$U c_{i\uparrow}^\dagger c_{i\uparrow} c_{i\downarrow}^\dagger c_{i\downarrow} \approx \Delta c_{i\uparrow} c_{i\downarrow} + h.c$$
$\Delta \sim <c_{i\uparrow}^\dagger c_{i\downarrow}^\dagger>$ is the superconducting order. This is a s-wave superconducting order which is uniform in momentum space when we do Fourier transform. 

If we have a Hamiltonian $H \sim \Delta c_{i\uparrow} c_{i\downarrow} + h.c$, then we understand that this term destroys (creates if $c_{i\uparrow}^\dagger c_{i\downarrow}^\dagger$) two electrons. This means that this state cannot have constant number of electrons.
$$H|GS> = E_{GS} |GS>$$
The ground state($|GS>$) cannot have a well-defined number of electrons.
$$|GS>  \sim |2e> + |4e> + |6e> + \cdots$$
$$|GS> \sim |1e> + |3e> + |5e> + \cdots$$

## How does superconducting order ($\Delta = <c_{i\uparrow}^\dagger c_{i\downarrow}^\dagger>$ ) transform under a gauge transformation? 

The phases do not cancel out, instead it adds up($\Delta \rightarrow e^{-2i\phi}\Delta$). Superconducting order is an order parameter which changes under gauge transformation. Hence superconductivity breaks [[Gauge Symmetry]]. Under [[Nambu representation]] a superconducting gap opens up for a non-zero $\Delta$. 

## Impact of [[Superconductivity]] in the electronic structure 

The following images show the electronic structure for triangular lattice for a varying chemical potential($\mu$). 

For $\Delta = 0$
![[triangular-lattice-delta_0.png]]

For $\Delta = 0.5$
![[triangular-lattice-delta_0.5.png]]

A non-zero uniform (in momentum space) superconducting order parameter will always open a gap with same magnitude, irrespective of what the chemical potential is or how does the dispersion looks like. 

## Gapped and gapless superconductivity 

The electronic structure is modified differently depending on the type of superconductivity. 
![[types-of_SC.png]]
