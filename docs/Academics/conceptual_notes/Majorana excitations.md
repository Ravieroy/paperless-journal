 
We consider the following Hamiltonian written in [[Nambu representation]], 

$$H =\Psi_k^\dagger \mathcal{H}\Psi_k$$

with a Nambu spinor defined as

$$\Psi_k = \left\lbrack \matrix{c_{k\uparrow} \cr c_{k\downarrow} \cr c_{-k\downarrow}^\dagger \cr -c_{-k\uparrow}} \right\rbrack
$$

Where, 

$$\mathcal{H} = \left\lbrack \matrix{\epsilon_k & 0 & \Delta & 0 \cr 0 & \epsilon_k & 0 & \Delta \cr \Delta & 0 & -\epsilon_k & 0 \cr 0 & \Delta & 0 & \epsilon_k} \right\rbrack
$$

???+ note "Majorana Fermion"
	It is a very special type of fermion which is by definition it's own antiparticle($\Psi^\dagger = \Psi$). These particles do not appear naturally in materials, as we only have electrons.


Mathematically, each electron can be written as two Majoranas

$$c = \Psi_\alpha + i\Psi_\beta, c^\dagger = \Psi_\alpha - i\Psi_\beta$$

$$\Psi_\alpha^\dagger = \Psi_\alpha, \Psi_\beta^\dagger = \Psi_\beta$$

!!! tip "Questions"
	- Can we isolate a single Majorana in materials?
	- Can we have superconductors in nature that show these excitations?

## Minimal model for 1D topological superconductor 

One dimensional spinless p-wave superconductor(Kitaev model)

$$H = \sum_n tc_{n+1}^\dagger c_n + \Delta c_n c_{n+1} + c.c$$

Where, $c_k = \sum_n e^{ikn} c_n$ and $\Delta(k) = -\Delta(-k)$
After Fourier transform, we have

$$H = \sum_k \epsilon_k c_k^\dagger c_k + i \Delta[c_{-k}c_k \sin k - c_{-k}^\dagger c_k^\dagger \sin k]$$

Spinless fermions in a 1D chain, (hopping and superconducting order are equal)

$$H = \sum_n c_{n+1}^\dagger c_n + c_n c_{n+1} + h.c$$

can be transformed into ($\gamma$ are Majorana operators)

$$H = i\sum_n \gamma_{2n}\gamma_{2n+1}$$

$c_n = \gamma_{2n-1} + i \gamma_{2n}$

![[majorana.png]]

At the ends of the chain there are zero energy excitations in the superconducting state. 
