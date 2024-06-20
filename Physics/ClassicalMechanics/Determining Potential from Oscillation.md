---
aliases: [determining potential from oscillation]
---

#ClassicalMechanics 
#NotHappyWithExplanation 

We know from [[Motion in One Dimension|motion in one dimension]] how to calculate the period of an oscillation given a potential. We ask, what if we knew the period of oscillation? Then could we determine the potential?

Suppoe in the reigon of space we consider the potential $U$ only has one minimum. Furthermore, we take the origin of the coordinate system to be at the minimum. The integral for period can be rewritten as 

$$
T = \sqrt{2m}\int\frac{dx}{\sqrt{E-U}} = \sqrt{2m}\int\frac{dx}{dU}\frac{dU}{\sqrt{E-U}}
$$
where we interpret $x$ as a function of $U$. However, since the potential has quadratic structure (because we know the system is oscillating) the function $x(U)$ is doubled valued. Therefore we have split the function into two regimes one for $x_1(U)$ for $x<0$ and $x_2(U)$ for $x>0$. Then the integral becomes
$$
T = \sqrt{2m}\int\frac{dx}{dU}\frac{dU}{\sqrt{E-U}} = \sqrt{2m}\left[\int_E^0\frac{dx_1}{dU}\frac{dU}{\sqrt{E-U}}+\int^E_0\frac{dx_2}{dU}\frac{dU}{\sqrt{E-U}}\right]
$$
$$
T =\sqrt{2m}\left[\int^E_0\left(\frac{dx_2}{dU}-\frac{dx_1}{dU}\right)\frac{dU}{\sqrt{E-U}}\right].
$$

Then divide both sides by $\sqrt{\alpha-E}$ where we integrate $E$ from 0 to $\alpha$ giving

$$
\int_0^{\alpha}\frac{T(E)dE}{\sqrt{\alpha-E}} = \sqrt{2m}\int_0^{\alpha}\int^E_0\left(\frac{dx_2}{dU}-\frac{dx_1}{dU}\right)\frac{dUdE}{\sqrt{\alpha-E}\sqrt{E-U}}.
$$
Switching the order of integration gives
$$
\int_0^{\alpha}\frac{T(E)dE}{\sqrt{\alpha-E}} = \sqrt{2m}\int^{\alpha}_0\left(\frac{dx_2}{dU}-\frac{dx_1}{dU}\right)dU\int^{\alpha}_{U}\frac{dE}{\sqrt{\alpha-E}\sqrt{E-U}}
$$
***not sure how he gets the boundaries?***. Essentially the integral over $E$ is equal to $\sqrt{\pi}$ and the integral over $U$ gives $x_2(U)-x_1(U)$ since $x_2(0)=x_1(0)=0$. This means that 

$$
x_2(U)-x_1(U) =\frac{1}{\pi\sqrt{2m}} \int_0^{\alpha}\frac{T(E)dE}{\sqrt{\alpha-E}}.
$$

So far we can only compute the different between two points, but cannot get a proper function $x(U)$. If we know that $U$ is symmetric about its axis then $x_1(U) = -x_2(U)$. Which implies

$$
x(U) = \frac{1}{2\pi\sqrt{2m}} \int_0^{\alpha}\frac{T(E)dE}{\sqrt{\alpha-E}}.
$$