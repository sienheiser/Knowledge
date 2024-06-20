
## Abstract
We have constructed the fibre bundle $(\mathit{C}^1\times\mathbb{R},\pi,\mathit{C}^1)$ [[Making a Fibre Bundle|here]]. In this note we make it into a Principal G-bundle by 
1. Defining an action of a Lie group on $\mathit{C}^1\times\mathbb{R}$
2. Showing that it satifies the definition of a [[Principal G-bundle|principal G-bundle]].

## Choice of action

If we look at $\mathit{C}^1\times\mathbb{R}$ there are two symmetries
1. The circle symmetry
2. The line symmetry or translation along a line
This means there are two possible actions we can define. 

## Circle symmetry

Let's start by using the circle symmetry. We know the group $SO(1)$ is the rotation of a circle. We can take an element $g(\theta)\in SO(1)$ which rotates a point $p\in\mathit{C}^1$ by $\theta$.  We can use the [[Making a Bundle#Charts|cartesian chart]] to define the action of $g(\theta)$ on a point. 

Take a point $p\in\mathit{C}^1\times\mathbb{R}$. Then define the right action of $g(\theta)$ on $x_{\mathit{C}^1\times\mathbb{R}}(p)$ as
$$
\begin{aligned}
	x_{\mathit{C}^1\times\mathbb{R}}(p)\triangleleft g(\theta) &= (r\cos a,r\sin a,b)\triangleleft g(\theta)\\
	&= (r\cos a\cos\theta-r\sin a\sin \theta,r\cos a\sin\theta+r\sin a\sin\theta,b)\\
	&= (r\cos(a+\theta),r\sin(a+\theta),b).
\end{aligned}
$$

### Checking if it is a principal SO(1)-Bundle
Now that we have a right action we can check if we have a Principal SO(1)-Bundle by checking if it satisfies the definition of [[Principal G-bundle|principal G-bundle]]. 

#### Right action space?

We check if $\mathit{C}^1\times\mathbb{R}$ with $SO(1)$ action is a [[Right G-action|right action space]] by checking if it satisfies the definiton of [[Right G-action]].

1. $\forall p\in \mathit{C}^1\times \mathbb{R}:p\triangleleft g(0) = p$? Where $g(0)\in SO(1)$ is the identity.
So 
$$
\begin{aligned}
x_{\mathit{C}^1\times\mathbb{R}}(p)\triangleleft g(\theta) &= (r\cos(a+\theta),r\sin(a+\theta),b).\\
\end{aligned}
$$
This is only equal to $x_{\mathit{C}^1\times\mathbb{R}}(p)$ if and only if $\theta=0$. There the action satisfies the first condition of the definiton

2. $\forall g(\alpha),g(\beta)\in SO(1):\forall p\in \mathit{C}^1\times\mathbb{R}: (p\triangleleft g(\alpha))\triangleleft g(\beta) = p\triangleleft(g(\alpha)\cdot g(\beta))$ 
We first check the LHS which
$$
\begin{aligned}
(x_{\mathit{C}^1\times\mathbb{R}}(p)\triangleleft g(\alpha))\triangleleft g(\beta) &= (r\cos(a+\alpha),r\sin(a+\alpha),b)\triangleleft g(\beta)\\
&= (r\cos(a+\alpha+\beta),r\sin(a+\alpha+\beta)).
\end{aligned}
$$

Then we check the RHS by first computing $g(\alpha)\cdot g(\beta)$. To do this we need to calculate $( $(g(\alpha)\cdot g(\beta))^i_j$ where $i,j=1,2$. This is essentially a matrix multiplication and we get 
$$
\begin{aligned}

(g(\alpha)\cdot g(\beta))^1_1 &= \cos(\alpha+\beta)\\	
(g(\alpha)\cdot g(\beta))^1_2 &= -\sin(\alpha+\beta)\\
(g(\alpha)\cdot g(\beta))^2_1 &= \sin(\alpha+\beta)\\
(g(\alpha)\cdot g(\beta))^2_2 &= \cos(\alpha+\beta)

\end{aligned}
$$
Therefore RHS is
$$
\begin{aligned}
	x_{\mathit{C^1}\times\mathbb{R}}(p)\triangleleft(g(\alpha)\cdot g(\beta)) &= (r\cos a\cos(\alpha+\beta)-r\sin a\sin(\alpha+\beta),r\cos a\sin(\alpha+\beta)+r\sin a\cos(\alpha+\beta),b)\\
	&= (r\cos(a+\alpha+\beta),r\sin(a+\alpha+\beta),b).
\end{aligned}
$$
Therefore the RHS = LHS.  So this is a right action space

#### Checking if the action is free
Now we need to show that the defined right action of $SO(1)$ on $\mathit{C}^1\times \mathbb{R}$ is [[Right G-action#Stablizers|free]]. Take any $g(\theta)\in SO(1)$. Then

$$
x_{\mathit{C}^1\times\mathbb{R}}(p)\triangleleft g(\theta) = (r\cos(a+\theta),r\sin(a+\theta),b).
$$
The only way we can get back $p$ is if $\theta = 0$. Therefore the action is free.

#### Checking if condition three is satified

Finally we check if the final condition of [[Principal G-bundle]] is satified. For this we need to constuct $\mathit{C^1}\times\mathbb{R}\backslash SO(1)$. Start with defining the [[Right G-action#Orbitals|orbit]] for all $p\in \mathit{C}^1\times \mathbb{R}$

$$
 \mathit{O}_p = \{q:\exists g\in SO(1)\quad q\triangleleft g = p\}.
$$
Notice that all the points that belong to $\mathit{O}_p$ lie on the circle that intersects through $p$. So the orbits in the case are circle. 

We can make orbits for other points that do not belong to $\mathit{O}_p$. We may choose points such that they all lie on the fibre $\text{preim}_\pi(\{p\})$. Because of the equivalence relation this is well defined. We can then construct the quotient space
$$
\mathit{C^1}\times\mathbb{R}\backslash SO(1)  =\{\mathit{O}_q:q\in \text{preim}_\pi(\{p\})\}.
$$
We define the projection $\mathit{C^1}\times\mathbb{R}\stackrel{\rho}{\longrightarrow} \mathit{C^1}\times\mathbb{R}\backslash SO(1)$ as 
$$
\forall p\in \mathit{C^1}\times\mathbb{R}:\rho(p) = \mathit{O}_q\quad \text{where }p\in\mathit{O}_q\in \mathit{C^1}\times\mathbb{R}\backslash SO(1).
$$
So have defined a bundle. Now we need to show that $\mathit{C^1}\times\mathbb{R}\stackrel{\pi}{\longrightarrow} \mathit{C^1}$ is bundle-morphic to $\mathit{C^1}\times\mathbb{R}\stackrel{\rho}{\longrightarrow} \mathit{C^1}\times\mathbb{R}\backslash SO(1)$. Notice that $C^1$ is a circle while $C^1\times\mathbb{R}\backslash SO(1)$ is a straight line. From a topological stand point a circle is not homeomorphic to a line. Therefore there does not exists a bundle-morphism between the two bundles. 

As a result the fibre-bundle $(C^1\times \mathbb{R},\pi,C^1)$ with the right action $SO(1)$ is not a principal $SO(1)-$bundle. However if we had the fibre bundle $(C^1\times\mathbb{R},\pi,\mathbb{R})$ where $C^1$ are the fibres. Then equiping this fibre bundle the right action $SO(1)$ would be a principal $SO(1)-$bundle.

### Conclusion
We start with a fibre bundle $(C^1\times \mathbb{R},\pi,C^1)$ and chose to define a $SO(1)$ right action on the fibre bundle, because of the circle symmetry present. Then we check whether this object is a [[Principal G-bundle]]. We find that the object satifies the first and second condition but does not satisfy the third condition, because the base spaces of $(C^1\times \mathbb{R},\pi,C^1)$ and $(C^1\times \mathbb{R},\rho,C^1\times\mathbb{R}\backslash SO(1))$ are not topologically homeomorphic. One is a circle and the other is a line.

If we want to define an $SO(1)$ principal bundle using $C^1\times\mathbb{R}$ as the total space. Then we need $\mathbb{R}$ to be the base space and $C^1$ to be the fibres of the fibre bundle. 

If we want to make $(C^1\times \mathbb{R},\pi,C^1)$ into a princial $G$-bundle where $G$ is some Lie group, then we have to choose an appropriate $G$. The most obvious choice of $G$ is the group of real number with addition as a group operation. In this case the orbitals would alse be the fibres and the quotient space would be a circle. This can be worked out explicitly and is left as an excersise to the reader.  

