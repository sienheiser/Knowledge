#StatisticalMechanics  
#NotHappyWithExplanation 


### Main Ideas

Coarse grain: Throw away information
Rescale: Zoom out 

### Example

We solve the 2D Ising model. Suppose we have a lattice of spin objects that can have either spin up or spin down. The Hamiltonian of such a system is given as

$$
H = -J \sum_{<ij>} S_i S_j.
$$

The partition function of the system is 

$$
Z = \sum_S e^{-\beta H(S)}
$$

where we sum over all the states. For example if we had three spin objects in a row, then there is a total of 8 states to sum over. Imagine the spins in the 2D grid are colored by either red or purple. Note these colours do not denote their spin. Start with coloring the spin on the top left of the grid as purple, then the next spin in the same row and column is coloured red. We continue to alternate the colours. Now we form another lattice only containing the red spins, and want to coarse grain the purple spins.


We rewrite the partitian function as two sums, one summing over all the red spins and the other summing over all purple spins

$$
Z = \sum_{S_{red}}\sum_{S_{purple}} \exp(-\beta H(S_{red},S_{purple})).
$$

We know have to guess the form of the new Hamiltonian. It must preserve the sysmmetry properties as the previous Hamiltonian. The new Hamiltonian has form

$$
\beta'H'(S_{red}) = -K'\sum_{<ij>} S_i S_j-L'\sum_{<<ij>>} S_i S_j - M'\sum_{unit cell}S_i S_j S_k S_l + H_0
$$

The first term corresponds to the neartest neighbour i.e. the diagonals. The second term correponds to the second nearest neighbours i.e. there existed a purple spin between two red spins.*** The second last term: not sure what the last term takes into account.*** Finally $H_0$ is an arbitrary constant.

The next thing is to equate the old and Hamiltonian, where we only compare the system in one unit cell. Then find the independent spin configurations of the system and solve $K'$, $L'$ and $M'$ in terms of $K$

