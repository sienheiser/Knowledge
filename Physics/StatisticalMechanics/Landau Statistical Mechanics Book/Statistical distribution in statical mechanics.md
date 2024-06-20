---
aliases: [statistical distribution]
---
#StatisticalMechanics 

### statistical distribution function
We know that it is not possible to keep track of every particle in a large system. Even if we focus on a [[Subsystems|subsystems]] of the large system. The interactions between the subsystem and the rest of the system are very complicated. However, due to the complexity another approach can be taken. 

Suppose we take a small volume element $\Delta q \Delta p$ in the phase space of the subsystem. Then as a long time $T$ passes. The phase trajectory of the subsystem passes through all possible states many times.  If we denote the $\Delta t$ as the time spent by the subsystem in states belonging to volume element  $\Delta q \Delta p$ and take $T$ to infinity. Then the ratio between $\Delta t$ and $T$ converge to a constant because the phase trajectory passes through volume many times (infinitely many times). We get the following relation

$$
w = \lim_{T\rightarrow\infty} \frac{\Delta t}{T}.
$$
The constant $w$ is the probability to find the subsystem in one of the states belonging to the volume element $\Delta q \Delta p$. If we take the infinitesimal limit of the volume element we get the infinitesimal volume element $dqdp$ (see [[volume element in phase space|volume element in phase space]]). We can define probability $dw$ of the state to be in volume element $dqdp$ as
$$
dw = \mathcal{Q(q,p)}dqdp.
$$
The function $\mathcal{Q}$ depends on all the generalized coordiantes and momenta of the system and it is called the statistical distribution function.

### properties of the distribution function

The integral over all phase space of the distribution funtion equals to one

$$
\int \mathcal{Q(q,p)}dqdp = 1.
$$

The distribution function of a given subsystem does not depend on the initial state of another small part of the same system. Furthermore, the distribution function does not depend on the initial state of the considered subsystem. 

The fundemental problem of statistical mechanics is finding the distribution function. This is because we can then calculate the mean value for any quantity $f(q,p)$ by $$\bar{f}=\int f(q,p)\mathcal{Q}(q,p)dqdp.$$ 
Interesting fact, if we could determing the quantity $f$ as a function of time then $$\bar{f}=\lim_{T\rightarrow\infty}\frac{1}{T}\int_0^T f(t)dt$$ 
this would exactly equvalent to mean being calculated by the distibution fucntion. We can see this from how we defined $w$ above.

