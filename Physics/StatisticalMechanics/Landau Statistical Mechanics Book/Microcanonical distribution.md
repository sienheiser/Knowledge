---
aliases: [microcanonical distribution]
---
#StatisticalMechanics 

### Microcanonical distribution
We can imagine a statistical distribution for a subsystem to be $\mathcal{Q} = constant$ for points in the phase space that represents subsystems with energy $E(q,p) = E_0$, momentum $\vec{P}(q,p) = \vec{P}_0$ and angular momentum $\vec{M}(q,p) = \vec{M}_0$. For the rest of the phase points that do not represent such a subsystem $\mathcal{Q} = 0$. Such a distribution function satisfies [[Louville's theorem]] trivially. This means that such a distribution is valid for a certain closed subsystem. If we want to normalize the distribution $\int \mathcal{Q}dqdp = 1$ we find that we need the distribution to be infinite at points where the energy $E(q,p) = E_0$, momentum $\vec{P}(q,p) = \vec{P}_0$ and angular momentum $\vec{M}(q,p) = \vec{M}_0$. To solve this problem we introduce [[Dirac delta functions]] into the distributions giving

$$
\mathcal{Q} = constant\times\delta(E(q,p)-E_0)\delta(\vec{P}(q,p)-\vec{P}_0)\delta(\vec{M}(q,p)-\vec{M}_0).
$$
Then it is possible to take the integral over all the phase space. The statistical distribution above is called a ***microcanonical distribution***

### Interesting fact
When restrict the system to only have $E(q,p) = E_0$, momentum $\vec{P}(q,p) = \vec{P}_0$ and angular momentum $\vec{M}(q,p) = \vec{M}_0$. The set of phase points that represent such subsystems forms a 2s-7 dimensional manifold in the phase space. I do not see why this is true?
 