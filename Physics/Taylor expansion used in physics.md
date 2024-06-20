---
aliases: [Taylor expansion in physics]
---

When deriving the conservation law of momentum and and the conservation law of angular momentum, we usually add an infinitesimal vector to the $\mathcal{L}$. For example in [[Momentum (Classical mechanics)#Momentum|momentum]] we add the same infinitesimal vector to all the radius vectors of the system. This means we shift the entire system by $\vec{\epsilon}$. Then we taylor expand Lagrangian to find the condition where that must not change the Lagrangian. 
In this article we will derive the scheme used. 

### expansion scheme
Suppose we have some function $f$ that takes in a position vector  $\vec{r}$ and returns a scalar. Suppose we add an infintesimal vector $\vec{\epsilon}$ to the position vector. The expansion of the function to first order  at  $\vec{\epsilon}=0$ is
$$
f(\vec{r}+\vec{\epsilon})=  f(\vec{r}) + \vec{\epsilon}\cdot \frac{\partial f(\vec{r}+\vec{\epsilon})}{\partial (\vec{r}+\vec{\epsilon})}\frac{\partial(\vec{r}+\vec{\epsilon})}{\partial \vec{\epsilon}}|_{\vec{\epsilon} = 0} = f(\vec{r}) + \vec{\epsilon}\cdot \frac{\partial f(\vec{r})}{\partial \vec{r}}
$$

We can also find the change in the function:
$$
\delta f = f(\vec{r}+\vec{\epsilon})-f(\vec{r}) =\vec{\epsilon}\cdot\frac{\partial f(\vec{r})}{\partial \vec{r}}
$$