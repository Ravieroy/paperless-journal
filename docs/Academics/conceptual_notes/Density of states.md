# Density of States
---
The density of states of a classical system is the number of states of that system per unit energy, expressed as a function of energy. This quantity may be formulated as a phase space integral in several ways. 

The most natural approach to the density of states is to find the volume of phase space corresponding to the shell defined by the energy range _E_ ≤ _H_(**q**, **p**) <$E+\epsilon$, and divide this by the span of the energy range $\epsilon$ before taking the limit $\epsilon \rightarrow 0$.

$\rho(E) = h^{-n} \text{lim}_{\epsilon \rightarrow 0} \frac{1}{\epsilon}\int 1_{E,E+\epsilon}(H(q,p))dqdp$

In which **1** is an indicator function, which is unity when its argument lies within the specified interval and zero elsewhere.

It is easy to see that the definition above is essentially a differential. It is therefore entirely equivalent to find the total number of states up to and including _E_ by a suitable phase space integral and then differentiate with respect to _E._


$\rho(E) = h^{-n} \frac{d}{dE}\int 1_{0,E}(H(q,p))dqdp$

It is sometimes convenient to do the same thing by using a Dirac delta function to project out the required value of the energy, for example

$\rho(E) = h^{-n} \int \delta(H(q,p)-E)dqdp$

From this last definition, it is easy to see that the density of states measures the number of states of the system per unit energy at the given energy.

![[DOS.png]]

---
!!! note "Useful Links :"
1. [Density of States - Engineering LibreTexts](https://eng.libretexts.org/Bookshelves/Materials_Science/Supplemental_Modules_(Materials_Science)/Electronic_Properties/Density_of_States)

