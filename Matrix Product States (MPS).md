---
aliases: [MPS]
---

#QuantumMechanics 
#NotHappyWithExplanation 


Consider a generic  many-body state formed by $L$-constituents that each have a local Hilbert space $\mathcal{H} = span\{|i\rangle, i = 1,....,d \}$. Then a state ket may be written as

$$
|\Psi\rangle = \sum_N C(i_1,....,i_L)|i_1,....,i_L\rangle
$$
where $C(i_1,....,i_L)$ are complex coefficients and $|i_1,....,i_L\rangle$ are the basis. It is clear that each $i_j$ has $d$ possible values. This means that we have $d^L$ possible configurations for the arguments of $C(i_1,....,i_L)$ which implies there are $d^L$ $C(i_1,....,i_L)$.  The main question to ask is if we can have a better representation.

What one can do is represent the $C(i)$ as a tensor with $L$ indices. Then using [[Generalized SVD (Graphical notation)]] we can redraw the tensor completely in terms of decomposed matrices as seen below
![[CoefficientSVD.png]]

The main idea in the above diagram is to group up $L-1$ indices using a bijective map and then performing SVD as in [[Graphical notation SVD]]. However this is done for all indices. In the above figure, SVD is performed between $i_1$ and $i_2, i_3,....,i_L$ then between $i_L$ and $i_1, i_2,....,i_{L-1}$ and we keep alternating until we reach to some center with a diagonal matrix (the second last equality). ***The notation in the last equality is unclear***. Then using the graphical notation for $C(i_1,i_2, i_3,....,i_L)$ for the state ket $|\Psi\rangle$ we get 

![[SchmidthDecomposition.png]]

What we have done is essentially a [[Schmidth decomposition]] of a state ket. 	
