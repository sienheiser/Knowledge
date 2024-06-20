#ClassicalMechanics 

Suppose we have a general system with $s$ degrees of freedom that has a stable minimum at $q_{i0}, q_{i1},....,q_{is}$. Then we may use the same scheme as in [[Harmonic Approximation 1D]]. That is set the zeroth order term to zero, the first order term of the potential goes is zero at the minimum and we leave the second order terms. The most general Lagrangian we get is 
$$
\mathcal{L} = \frac{1}{2}\sum_{i,j = 1}^{s} a(q)\dot{q}_i\dot{q}_j-k_{ij}q_i q_j \tag{1}
$$
where we can set $a(q)=a(q_{i0},q_{j0}) = m_{ij}$ we take it to be symmetric in the indices just like $k_{ij}$.

The general equation of motion for the $k$th variable is

$$
\sum_i m_{ik}\ddot{q}_i +k_{ik}q_i = 0 \tag{2}
$$

we can rewrite the above equation as in matrix form as

$$
M \ddot{\vec{R}} = K \vec{R} \tag{3}
$$
where
$$
M_{ik} = m_{ik}\quad, K_{ik} = k_{ik}. \tag{4}
$$
and $\vec{R} = [q_1,...,q_s]^T$. With the ansatz 

$$
\vec{R} = [A_1 \quad A_2 \quad ... \quad A_s]^{T} e^{i\omega t} = \vec{A}e^{i\omega t}. \tag{5}
$$
 
and plugging equation (5) into equation (3) we get 
$$
(K+\omega^2 M)\vec{A} = 0. \tag{6}
$$
Equation (6) is a system of equations. If there are non-zero intrinsic frequencies then det|$K+\omega^2 M$| = 0. Taking the determinant gives a polynomial equation of degree $s$ in terms of $\omega^2$. Solving for the roots of the polynomial equation gives $\omega^2_{\alpha}$ where $\alpha = 1,2,...,s$ and are positive in general. If any of these roots are not positive then would mean $\omega_k$ has imaginary component which when placed in the ansatz gives an exponential increase or decrease.

Once $\omega_{\alpha}$ are determined we can find the eigenvectors using equation (6). Once the normalized eigenvectors $\vec{e}_1,...,\vec{e}_s$ are found we may write $\vec{R}$ as a linear combination of these vectors

$$
\vec{R} = \sum_j C_{j}e^{i\omega_j t}\vec{e}_j = \sum_j \Theta_j \vec{e}_j. \tag{7}
$$

Therefore equation (7) can be written in component form

$$
q_k = \sum_j \Delta_{jk}C_{j}e^{i\omega_j t} = \sum_j \Delta_{jk}\Theta_j. \tag{8} 
$$
where $\Delta_{jk}$ is the $k$th component of the $j$th eigenvector. Each of these new $\Theta_i$ coordinates are indepenent of each other so they satisfy the following equation of motion

$$
\ddot{\Theta_i} + \omega_i^2\Theta_i = 0. \tag{9}
$$





