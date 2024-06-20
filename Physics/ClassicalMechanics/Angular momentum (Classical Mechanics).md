---
aliases: [angular momentum, conservation of angular momentum, angular momentum conservation]
---
#ClassicalMechanics 

### Angular momentum
We know that space is isotropic. Therefore, when we rotate the entire system, the Lagrangian should stay the same. We will derive the condition for the Lagrangian to stay the same by rotating the system infinitesimally. 
Let the system be defined by set of position vectors $\vec{r}_a$ this means that the velocity vectors $\vec{v}_a$ can also be defined. Suppose we rotate all the position vectors about the axis of an infinitesimal vector $\vec{\delta \phi}$ with magnitude $\delta\phi$.  Infinitesimally rotating vectors can be described linearly. If we choose $\vec{\delta r}=\vec{\delta \phi}\times\vec{r}$, then define $\vec{r}^{'} =\vec{r}+\vec{\delta r}$. The vector $\vec{r}^{'}$ is the new rotated vector (remember our coordinate system stays the same). The velocity vectors also get rotated by the same amount, so $\delta\vec{v} = \vec{\delta \phi}\times\vec{v}$. Now we have our $\mathcal{L}(\vec{r},\vec{v})$ become $\mathcal{L}(\vec{r}+\vec{\delta r},\vec{v}+\vec{\delta v})$. Using the scheme set up in [[Taylor expansion used in physics#expansion scheme|Taylor expansion in physics]] we get

$$
\delta\mathcal{L} = \sum_a \vec{\delta\vec{r}_a}\cdot\frac{\partial \mathcal{L}(\vec{r}_a,\vec{v}_a)}{\partial \vec{r}_a} + \vec{\delta\vec{v}_a}\cdot\frac{\partial \mathcal{L}(\vec{r}_a,\vec{v}_a)}{\partial \vec{v}_a}
$$
where we expanded at $\vec{\delta r_a} = \vec{\delta v_a}=\vec{0}$. We can rewrite  $\frac{\partial \mathcal{L}(\vec{r}_a,\vec{v}_a)}{\partial \vec{r}_a} = \dot{\vec{p}}_a$ and $\frac{\partial \mathcal{L}(\vec{r}_a,\vec{v}_a)}{\partial \vec{v}_a} = \vec{p}_a$ Then if we substitude the definition of $\vec{\delta r_a}$ and $\vec{\delta v_a}$ into the expansion we get

$$
\delta\mathcal{L} = \sum_a (\vec{\delta \phi}\times\vec{r}_a)\cdot\dot{\vec{p}}_a +(\vec{\delta \phi}\times\vec{v}_a)\cdot\vec{p}_a =  \sum_a [\vec{r}_a\times\dot{\vec{p}}_a +\vec{v}_a\times\vec{p}_a]\cdot \vec{\delta \phi} = \sum_a\vec{\delta \phi}\cdot \frac {d}{dt}[\vec{r}_a\times\vec{p}_a].
$$

This means that for the Lagrangian to not change we have $\frac {d}{dt}\sum_a \vec{r}_a\times\vec{p}_a=0$. We define the total angluar momentum of the system to be 

$$
\vec{M} = \sum_a \vec{r}_a\times\vec{p}_a
$$
and it is conserved in a closed system. 

### transformation law of angular momentum
Suppose we have two radius vectors $\vec{r}$ and $\vec{r}^{'}$ pointing at the same point. Let the distance between the two origins be given by $\vec{a}$. Then
$$
\vec{r} = \vec{r}^{'}+\vec{a}.
$$
Pluging the above formula into the formula for gives 
$$
M = \sum_a (\vec{r}^{'}_a+\vec{a})\times\vec{p}_a = \vec{M}^{'}+\vec{a}\times\vec{P}.
$$
The above equation shows that angular momentum depends on point of origin unless $\vec{P}$ is zero.

Suppose we have two frames $K$ and $K^{'}$ where $K^{'}$ is moving with velocity $\vec{V}$ w.r.t $K$. Then we can use the relation between radius vectors of the two frames and velocity vectors of the two frame. A short can be used, where we can imagine that the two frames conincide at a certain time. Then the radius vectors are the same. But the velocity vectors are given by $\vec{v} = \vec{v}^{'}+\vec{V}$ which is true even after the two frames no longer coincide.  Plugging this into formula for $\vec{M}$ gives
$$
M = \sum_a m_a\vec{r}_a\times(\vec{v}^{'}_a+\vec{V}) = \vec{M}^{'}+ \sum_a m_a\vec{r}_a\times \vec{V} = \vec{M}^{'}+\mu\vec{R}\times \vec{V}.
$$
If the moving frame is the rest frame for the system then the $\vec{V}$ is the velovity of the center of mass of the system. This means that $\mu\vec{V} = \vec{P}$. Therefore 
$$
M = \vec{M}^{'}+\vec{R}\times \vec{P}.
$$
The above equations shows that a system has its intrinsic angular momentum and another angular momentum term due to its overall motion.