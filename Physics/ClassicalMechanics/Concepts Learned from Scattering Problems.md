#ClassicalMechanics 
We have derives the effective scattering cross section in [[Scattering (CM)]]. I gone through the problems for unit 18 in Landau's book. These are the main ideas that I learned from solving the problem.

1. Problem 1: The effective scattering cross section in [[Scattering (CM)]] is only for the center of mass frame. Computing for the potential given in problem 1 is simple. To jump to the lab frame we have to use relations between the C-frame and L-frame derived in [[Elastic Collisions (L frame)]] more specifcally equation 16.6 in the book. Consider all the cases, i.e. $m_1 > m_2$, $m_1 < m_2$ and $m_1 = m_2$.
2. Problem 2:  Here we use the effective scattering cross section computed in problem 1 and changing it dependency from particles scattered between angles $\chi$ and $\chi + d\chi$ to particles scattered with energies $E$ and $E+dE$. The scattering potential for problem 1 is 
$$
d\sigma =  	\frac{1}{2}\pi a^2 \sin\chi d\chi.
$$

Assuming particle mass $m_2$ is at rest and particle with mass $m_1$ has initial velocity $v_{\infty}$. After the collision in the lab frame $m_2$ will have velocity
$$
v_2' = \frac{2m_1v_{\infty}}{m_1+m_2}\sin(\frac{\chi}{2})
$$
meaning it has gained energy and $m_1$ has lost energy. We can rewrite the above equation in terms of $\cos(\chi)$ and initial energy of the first particle. The final answer should be 
$$
d\sigma = \frac{a^2\pi}{\epsilon_{max}}d\epsilon
$$
where $\epsilon_{max} = 2m_2 m_1/(m_1+m_2)^2 E_1$ and $E_1 = 1/2 m_1 v_{\infty}$.

3. Problem 3: Using mechanical similarity we may find the relation between impact parameter $\rho$ and $v_{\infty}$. Furthermore, for similar paths the angles remain exactly the same this can be proven using the angle integration formula. Since we know relation between $\rho$ and $v_{\infty}$ then we can find relation between $d\sigma$ and $v_{\infty}$.
4. Problem 4: The main idea is to find for a fixed velocity $v_{\infty}$ the maximum value of the impact parameter $\rho$ for which the particle will fall to the center. Try drawing the graph of the effective potential and see for which energies is the particle able to reach the center. Then we know that total scattering cross section  for particle to fall to the center is $\sigma = \pi \rho_{max}$.
5. Problem 5 and Problem 6 similar to problem 4.
6.  Problem 5 and Problem 6 are similar to problem 4. They differ on how to find the max value of the impact parameter.