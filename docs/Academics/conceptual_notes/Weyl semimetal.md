## Weyl Semimetals 
Tags: #weyl_nodes

### Basic Hamiltonian and Properties 

An analogous situation of [[Weyl fermions]] prevails in 3+1 dimensions. The gamma matrices are, as Dirac found, now 4 × 4 matrices and can be represented as $\gamma^0 = \mathcal{I}^{2 \times 2} \otimes \tau_x$,  $\gamma^i = \sigma^i \otimes i\tau_y$ and $\gamma^5 = -\mathcal{I}^{2 \times 2} \otimes i\tau_z$.  Again, if we
identify chiral components $\gamma_5 \psi_\pm = \pm\psi_\pm$, where $\psi_\pm$ are effectively two component vectors, we have for the massless Dirac equation
$$i\partial_t\psi_\pm = H\pm\psi_\pm$$
$$H_\pm = \mp\vec{p} \cdot \vec{\sigma}$$
Thus Weyl fermions propagate parallel (or antiparallel) to their spin, which defines their chirality. We will see that a single chirality of Weyl fermions cannot be realized in 3D, but momentum separated pairs can arise. These are the Weyl semimetals.

These are three-dimensional topological phases of matter with strong spin-orbit coupling. They are featured by pairs of linear band crossings, called Weyl nodes, in
momentum space. Since the Weyl nodes are topologically protected and closely associated with the [[Chiral Anomaly]], WSMs impose a plethora of characteristic phenomena, such as surface Fermi arcs, nonlocal transport, and anomalous magnetoconductance.

In principle, Weyl nodes of opposite [[Chirality]] do not need to have the same electron population. An electron population imbalance between Weyl nodes of different [[Chirality]], called [[Chiral Chemical Potential]] can be achieved, e.g. by the chiral anomaly with applying parallel electric and magnetic fields, by a strain deformation or in a superlattice system with breaking both [[Time reversal symmetry]] and inversion symmetries. 

---

### Topological aspects of WSM 
In Weyl semimetals, the conduction and valence bands coincide in energy over some region of the Brillouin zone. Furthermore, this band touching(*determined by symmetry*) is stable at least to small
variations of parameters(interaction or disorder). 
- This could be because disorder is average and on average keeps the symmetry
- Band structure of semimetal has very low density of states on the Fermi level 

>**Spin rotation symmetry (*ignore spin-orbit coupling*) :** Bands are doubly degenerate. 
>**Both [[Time reversal symmetry]] ($\mathcal{T}$) and inversion symmetry:** Bands are doubly degenerate. Crystal momenta are invariant. 
>**Only $\mathcal{T}$ is present :** Band is non-degenerate, as crystal momentum is reversed under its action. At $\textbf{k} = -\textbf{k}$ which is TRIM, there is a Kramer's degeneracy([[Kramers Theorem]]) present. 
> **$\mathcal{T}$ is broken, and only inversion is present :** Bands are typically non-degenerate.

$\mathcal{T}$ is broken, and only inversion is present$\mathcal{T}$ is broken and only inversion is present

$$H = f_0 \mathcal{I}^{2 \times 2} + f_1\sigma_x + f_2\sigma_y + f_3\sigma_z$$
To bring the bands in coincidence we need to adjust all three coefficients $f_1 =f_2 =f_3 =0$ simultaneously, which requires three independent variables, i.e. we are in 3D. As we can then expect band touchings without any special fine-tuning, we
can readily argue that the existence of Weyl nodes is stable to small perturbations of Hamiltonian parameters.

$f_1(\textbf{k})$ typically vanishes in the momentum space. Typically, this is a 2D surface.  If we
demand a simultaneous zero of $f_2(\textbf{k})$ and $f_3(\textbf{k})$, this specifies the intersection of three independent surfaces, which typically occurs at a point.  Consider a perturbation that changes the functions by a small amount. This will also move the zero surfaces and their points of intersection by a small amount, but the intersection will persist, just at a different crystal momentum. The Weyl nodes cannot be removed by any small
perturbation and may disappear only by annihilation with another Weyl node.

![[3D_intersection.png | 400x250]]

### Hamiltonian 
$$H = v\tau_x\mathbf(\sigma\cdot \textbf{k}) + m \tau_z + b\sigma_z +b^\prime \tau_z\sigma_x$$
$$
   H=
  \left( {\begin{array}{cc}
   m\mathcal{I}^{2\times2} + b\sigma_z +b^\prime \tau_z\sigma_x & v\mathbf(\sigma\cdot \textbf{k}) \\
   v\mathbf(\sigma\cdot \textbf{k}) & -m\mathcal{I}^{2\times2} + b\sigma_z - b^\prime \tau_z\sigma_x \\
  \end{array} } \right)
$$
Where, $\textbf{k} =(k_x,k_y,k_z)$ and $\tau_n$'s are Pauli Matrices for the pseudospin orbital degrees of freedom. m is a mass parameter, $b$ and $b^\prime$ are Zeeman field that  physically can correspond to magnetic fields in the z and x directions, respectively

### Inversion symmetry breaking WSMs
For these kinds of WSMs the anomalous Hall conductivity vanishes due to presence of $\mathcal{T}$ symmetry. 