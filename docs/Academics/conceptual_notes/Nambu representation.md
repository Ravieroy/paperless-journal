We have the Hamiltonian, 

$$H = \sum_{k,s} \epsilon_k c_{k,s}^\dagger c_{k,s} + \sum_k \Delta c_{k\uparrow}^\dagger c_{-k\downarrow}^\dagger + h.c$$


We define a Nambu spinor, 

$$\Psi_k = \left\lbrack \matrix{c_{k\uparrow} \cr c_{k\downarrow} \cr c_{-k\downarrow}^\dagger \cr -c_{-k\uparrow}} \right\rbrack
$$

Hence, the Hamiltonian in the Nambu basis is quadratic and can be diagonalized. The original Hamiltonian then can be written as,

$$H =\frac12 \Psi_k^\dagger \mathcal{H}\Psi_k$$

Where, 

$$\mathcal{H} = \left\lbrack \matrix{\epsilon_k & 0 & \Delta & 0 \cr 0 & \epsilon_k & 0 & \Delta \cr \Delta & 0 & -\epsilon_k & 0 \cr 0 & \Delta & 0 & \epsilon_k} \right\rbrack
$$

We have doubled the degrees of freedom. 

## Nambu electronic structure
### How the electronic structure is represented in the Nambu basis?

The single orbital in the square lattice is represented by the above Hamiltonian H. The following figure shows the electronic structure with and without the Nambu spinor ($\Delta = 0$).
![[nambu-square.png]]

A superconducting gap in the single particle electronic spectra opens at the Fermi level when a non-zero $\Delta$ is chosen.  This is a [[BdG]] band structure which has a hole and electron parts. 
![[nambu-square-sc.png]]

