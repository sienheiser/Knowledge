---
aliases: [motion in one dimension]
---
#ClassicalMechanics 

The most general form of a one dimensional Lagrangian is 
$$
\mathcal{L} = \frac{1}{2}a(q)\dot{q}^2+U(q)
$$
in Cartesian coordinates it becomes

$$
\mathcal{L} = \frac{1}{2}m\dot{x}^2+U(x).
$$

One can get relations between time $t$ and $x$ from the conservation of energy rather than the E-L equations. We know from [[Energy|energy]] that $E = T+ U$. That is if we translate through time and the Lagrangian remains the same, then energy is conserved (***Does this mean that as long as Langrangian does not depend on time energy is always conserved?***). We can get the following equation
$$
\frac{2}{m}(E-U(x)) = \left(\frac{dx}{dt}\right)^2\implies t = \sqrt{\frac{m}{2}}\int \frac{dx}{\sqrt{E-U(x)}}.
$$

When solving for conventional equations of motion we obtain a constant everytime we integrate. In this case, those constant go into $E$. 

We know that kinetic energy is always positive. This means that generally $E$ is greater than $U(x)$. As result, motion is only perimented in reigons where $E\geq U(x)$.

![[AllowedMotionPotential.jpg]]

The above figure plots a pontential. The red line shows where the potential and the energt $E$ of the system are equal. The blue shaded reigons are the regions where motion is allowed. There are two types of motions, bounded and unbounded. The bounded motion is possible on the left shaded reigon, while the unbounded motion is possible on the right shaded reigon.
