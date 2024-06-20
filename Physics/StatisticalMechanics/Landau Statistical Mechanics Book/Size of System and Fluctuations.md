---
aliases:[proof 1]
---
#StatisticalMechanics 

We are going to show that as a system size increases physical quantities $f$ of the system decreses. First we note that most physical quantites $f$ that we are interested are additive. This is because the subsystems are [[quasi-closed system|quasi-closed systems]]. As an example, the internal energy of each subsystem compared to the interaction it does with other subsystem is large. So the internal energies of the whole system is just the sum of the individual subsystems.

With that we can define the quantity $f$ as

$$
f = \sum_{i=1}^N f_i,
$$
where $f$ is the physical quantity for the whole system and $f_i$ is the physical quantity the [[Subsystems|subsystems]]. The mean value of the system is

$$
\bar{f} = \overline{\sum_{i=1}^N f_i} = \sum_{i=1}^N \overline{f_i}.
$$
As the number of subsystem increases so does the mean value meaning that the mean value is directly proportional to the number of subsystems.

Then if we take the [[Standard deviation|variance]] of the qunatity $f$ we get
$$
\overline{(\Delta{f})^2} = \overline{\left(\sum_{i=1}^N \Delta f_i\right)^2}=\overline{\sum_{i=1}^N \sum_{j=1}^N\Delta f_i \Delta f_j}.
$$
The terms $\Delta f_i\Delta f_j = 0$ with $i\neq j$ becaue the mean  of $\Delta f_i = 0$. This means

$$
\overline{(\Delta{f})^2} = \sum_{i=1}^N\overline{(\Delta f_i)^2}.
$$
Here we see that the [[Standard deviation|variance]] is also proportional to the number of subsystems in the system. As a result the relative fluctuations

$$
\frac{\sqrt(\overline{\Delta f^2})}{\bar{f}} \approx \frac{1}{\sqrt{N}}.
$$

For additive $f$ quantities the relative fluctuations will decrease as the size of the system increases. 