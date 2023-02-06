# Fermi level 
---

>Read this in analogous with the [[Fermi energy]] for complete understanding. Also read the common[[Fermi level#Confusing aspects of Fermi Level | misconception]] regarding the Fermi level.

The Fermi level is the energy (not necessarily corresponding to an actual energy level of the system) at which the occupation probability given by the Fermi-Dirac distribution is 1/2. The Fermi level of a metal at zero temperature is the same as the Fermi energy of that metal. This is not true for insulators, where the Fermi level lies inside the energy gap. If we refer to the [[Fermi energy]] as the Fermi level at zero temperature. With this definition, the Fermi energy does not need to coincide with an actual energy level of the system.(^^==See Useful Links==^^)

It determines the probability of electron occupancy at different energy levels. The closer the Fermi level is to the conduction band energy, the easier it will be for electrons in the valence band to transition into the conduction band. It is the energy level which is occupied by the highest electron orbital at 0 Kelvin (absolute zero temperature) and a parameter of the Fermi-Dirac distribution:

$f(E) = \frac{1}{1+e^{(E-E_F)/kT}}$

Where _T_ is the absolute temperature and _k_ is Boltzmann’s constant. This function gives the probability _f(E)_ of an electron to occupy a state with energy _E_. The distribution function value will have to be nonzero in the conduction band for electrical conductivity to be possible.

Impurities and temperature can affect the Fermi level. Introducing impurities to atoms will bring the Fermi level up and when it is brought high enough, part of the tail will go over to the conduction band. This makes it easier for electrons to travel to the conduction band, and thus conductivity will improve. From the distribution function, temperature directly influences how the energy states are occupied. The tail of the function also gets longer and wider at higher temperatures, stretching out to the conduction band.

![[Fermi_level.png]]


==It is to be noted that although the probability function has a value in the energy gap, there are no available energy states within the interval (hence energy gap, with zero density of states) and therefore no electrons populate the gap.== 



!!! important
	The Fermi level and [[Fermi energy]] are usually confusing terms and are often used interchangeably to refer to each other. Although both the terms are equal at absolute zero temperature, they are different at other temperatures.

## Position of Fermi level 

!!! question "What does it mean when the Fermi level lies in the band gap or instead in one of the bands?"
	- **Metals**: are very good conductors because the Fermi level lies inside one of the bands, meaning there's no energy gap to overcome for an electron in the valence band to pass on to the conduction band. Which explains why metals are populated by quasi-free electrons in the conduction band.
	- **Semi-metals**: Very similarly to metals, $E_F$ lies in one of the bands, but unlike metals, here the overlap between valence and conduction bands are very small. But still no gap!
	- **Semiconductors**: For semiconductors, there's a small energy gap between the two valence and conduction bands, the states in the gap are _not_ available to the electrons. So in order to have moving charge carriers, electrons and holes, the system first has to be heated up (excited, also possible with an applied E-field) in order to overcome the gap $E_g$ and be able to occupy the available states in the conduction band. $E_F$ ==lies in the gap for semiconductors==, which means occupied and unoccupied states in valence and conduction band respectively are energetically separated. 
	- **Insulators**: the energy gap between the two bands in so large, that it becomes very difficult to excite electrons towards the conduction band, hence their poor conductivity.


## Confusing aspects of Fermi Level
 Frequently, the Fermi level is wrongly defined as the energy of the most energetic occupied electron state in a system. This definition leads to errors as soon as we have discrete energy eigenstates, in other words, when there's a gap between the most energetic occupied state and the least energetic unoccupied state in the system. Whereas the correct definition is the chemical potential at T=0K, and will be halfway between the minimum of the conduction band and the maximum of the valence band.

---
!!! note "Useful Links :"
1. [What’s Fermi Level and why is it important| CircuitBread](https://www.circuitbread.com/ee-faq/whats-fermi-level-and-why-is-it-important-in-a-semiconductor)
2. [Relation between band structure, dispersion, density of states, and the Fermi energy and Fermi level - Physics Stack Exchange](https://physics.stackexchange.com/questions/218387/relation-between-band-structure-dispersion-density-of-states-and-the-fermi-en)
3. [condensed matter - What does Fermi level in the band gap mean? - Physics Stack Exchange](https://physics.stackexchange.com/questions/155606/what-does-fermi-level-in-the-band-gap-mean)










