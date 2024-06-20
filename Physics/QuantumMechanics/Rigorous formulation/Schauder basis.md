Suppose we have a Hilbert space
*Definiton:* A subset $S$ is called a Schauder basis if 
1. There exists a finite set of vectors $\{e_1,...,e_n\}$ which are linearly independent. 
2. For any $\psi\in\mathit{H}$ there exits countable subset ${e_1,e_2,...}\subseteq S$ and a sequence $\{\psi^i\}_{i = 1,2,...}$ such that $\psi = \sum_{n=1}^d \psi^n e_n$ if $|S|<\infty$ else $\psi = \sum_{n=1}^\infty \psi^n e_n$.
3. $S$ has to be the 'smallest' such set.

For this to be possible we need a notion of convergence and completeness which are built into Banach spaces. 

*Remark:* Can replace the 2nd condiation as so. For any subset $M\subseteq \mathit{H}$ the $\text{span}(M) =\{\text{finite linear combinations of elements of M}\}$. Then the span($S$) of Shauder basis is $\mathit{H} = \overline{\text{span}(S)}$ where the overline denotes the topological closure. 