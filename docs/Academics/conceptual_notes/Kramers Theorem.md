## Kramer's Theorem 

[Source](https://ashour.dev/Physics/Kramers+Theorem)

!!! note "Theorem"
	 For every energy eigenstate of a time-reversal symmetric system with half-integer total spin, there is at least one more eigenstate with the same energy. That is, every energy level is at least doubly degenerate if it has half-integer spin

### Proof 
For spin-1/2 systems, we have $\Theta^2 = -1$ where $\Theta$ is the time-reversal operator. In such a time-reversal invariant system, $|\psi\rangle$ and $\Theta |\psi\rangle$ have the same energy (since $[H,\Theta] =0$). Thus, if we can prove that these two states are different, then we will have proved Kramer's theorem since there will be two different states with the same energy!

> Let us assume the two states are the same, i.e,
> 
> $\Theta |\psi \rangle = e^{i\phi}|\psi\rangle, \phi \in \mathcal{R}.$
> 
> Then 
> $\Theta^2 = \Theta e^{i\phi}|\psi\rangle = e^{-i\phi}\Theta|\psi\rangle = e^{-i\phi}e^{i\phi}|\psi\rangle \Rightarrow \Theta^2 = 1 \Rightarrow\Leftarrow$
> 
> (Proof by contradiction)

### Solid-State Physics 
Consider a system with Bloch states $|n,\textbf{k},\sigma \rangle$ where n is the band index, $\textbf{k}$ is the crystal momentum and $\sigma$ is the spin. For any such state, there is another state $\Theta |n,\textbf{k},\sigma \rangle$ with the same energy.

$\Theta |n,\textbf{k},\sigma \rangle = |n,-\textbf{k},-\sigma \rangle$

(Note that we use a notation where there are two bands labeled by the same n, one with spin-up and one with spin-down). In general, such a Kramer's doublet are located at different momenta $\textbf{k}$ and $-\textbf{k}$.  For example, consider the system shown in Fig. 1 below.

![[Kramers.png]]

Fig 1: The band diagram in the first Brillouin zone of a spin-1/2 particle with time-reversal symmetry in 1-dimension. The yellow line shows a constant energy cut, with four states having the same energy. There are two Kramer's pairs here, denoted by yellow dots. There is one pair at $\alpha_{\pm}$ and another at $\beta_{\pm}$.  These points are known as time-reversal conjugate momenta. Moreover, note the special green points at the center and the boundary of the zone (denoted by green dots), which are their own time-reversal conjugates. These points are known as the time-reversal invariant moment (TRIM).

---
