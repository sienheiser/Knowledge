---
aliases: [integrals of the motion]
---
#ClassicalMechanics 
### integrals of the motion

*Definition*: Suppose a system has 2$s$ quantities $q_i$ and $\dot{q}_i$ to describe its motion. The function of these quantities that remain constant during the motion of the system are called **integrals of the motion**.

When we place a Lagrangian in the [[Euler-Lagrange Equations|EL-equations]] we get $s$ equations of motion for a system with 2$s$ quantities. Essentially, when we integrate these equations of motion, the integration has to be done twice. As a result two constants needs to be introduced for each equation of motion.  In principle we could write these constanst in terms of the generalized coordiantes and velocities. These are the functions that are called integral of the motion.

*Fact*: Number of integrals of the motion for a clsed mechanical system with s degree of freedoms is 2s-1.

*Example*: Suppose we throw a ball with mass m in uniform gravitational field. Suppose the initial velocity has components in $x$ and $y$ direction. Then the Lagrangian is $\mathcal{L} = \frac{1}{2}m(\dot{x}^2+\dot{y}^2)-mgy$. The equations of motion are $\ddot{x} = 0$ and $\ddot y = -g$. After integrating twice we get $x = At+B$ and $y = -gt^2/2+Ct+D$. However if we choose another origin of time suppose $t = t-t_0$. Then we get $x = A(t-t_0)+B$ and $y = -g(t-t_0)^2/2+C(t-t_0)+D$. Then for example if we choose $t_0 = D/C$ we essentially eliminate one of the constants. So instead we have three constants instead of four constants.

*Proof*: Given $s$ equations of motion, we get $2s$ integration constants. We have the ability to set the origin of time somewhere else which means that we can choose t = t-t_0. The t_0 can be chosen such that it eliminates one of the integration constants.

Integrals of the motion do not have any physical significance