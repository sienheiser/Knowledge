q![[Exercise221.png]]
(i). Tried using direct algebraic computations, but could not prove it. We know that $r = \sqrt{a^2+b^2}\implies a,b\leq r$. Therefore if we take
$$
\lim_{r\rightarrow 0}||\langle a\pm\frac{1-r}{8},b\pm \frac{1-r}{8}\rangle||^2 = ||\langle \frac{1}{8},\frac{1}{8}\rangle||^2 = \frac{1}{32}.
$$
So we have found the lower bound of the magnitude. We look at the upper bound of the magnitude by taking 
$$
\lim_{r\rightarrow 1}||\langle a\pm\frac{1-r}{8},b\pm \frac{1-r}{8}\rangle||^2 = ||\langle a,b\rangle||^2\stackrel{1}{<} 1
$$
where $\stackrel{1}{<}$ is true by definiton of $a,b$. So we have shown that the upper bound is less than $1$, therefore
$$
\langle a\pm\frac{1-r}{8},b\pm \frac{1-r}{8}\rangle\in D
$$
which implies that $R_{\langle a,b\rangle}\subset D$.

(ii). To show the equality we need to show any $\langle x,y\rangle\in D$ also belongs to $\langle x,y\rangle\in\bigcup_{\langle a,b\rangle\in D}R_{\langle a, b\rangle}$. And any $\langle x,y\rangle\in\bigcup_{\langle a,b\rangle\in D}R_{\langle a, b\rangle}$ also belongs to $\langle x,y\rangle\in D$.

Take any $\langle x,y\rangle\in D$ then we know by definiton that 
$$
\langle x,y\rangle\in R_{\langle x,y\rangle}.
$$
Therefore 
$$
\langle x, y\rangle\in\bigcup_{\langle a,b\rangle\in D} R_{\langle a, b \rangle}.
$$


Now take any $\langle u, v\rangle$ such that 
$$
\langle u, v\rangle\in\bigcup_{\langle a,b\rangle\in D} R_{\langle a, b \rangle}.
$$
Then we know that $\langle u,v\rangle\in R_{\langle u, v\rangle}\stackrel{1}{\subset} D$ where $\stackrel{1}{\subset}$ is true because of (i). Therefore 
$$
D = \bigcup_{\langle a, b \rangle\in D}R_{\langle a, b \rangle}.
$$

(iii). We know that open rectangles are open sets in $\mathbb{R}^2$. All we have to do is show that $D$ is a  union of these rectangular open sets. 

We have shown in (iii) that
$$
D = \bigcup_{\langle a, b \rangle\in D}R_{\langle a, b \rangle}.
$$
therefore $D$ is a union of open sets which means $D$ is an open set.

(iv) Define points
$$
f(x,y)=\langle x\pm \frac{c-\sqrt{(x-a)^2+(y-b)^2}}{8},y\pm\frac{c-\sqrt{(x-a)^2+(y-b)^2}}{8} \rangle
$$
for $\langle x,y\rangle\in D$. 

Then if $x=a,y=b$ we get
$$
f(x,y) = \langle a , b \rangle+\frac{c}{8}\langle 1, 1\rangle.
$$
Clearly this point is in the circle with center $\langle a,b\rangle$ and radius $c$. Now take 
$$
\lim_{\sqrt{(x-a)^2+(y-b)^2}\rightarrow c} f(x,y) = \langle x, y \rangle\in D
$$
because the verticies converge to the point as we go to the boundary. Therefore $D_{\langle x, y\rangle}\subset D$ for $\langle x,y\rangle\in D$.



![[Exercise222.png]]
(i). Define sets 
$$
\begin{aligned}
D_1 &= \{\langle x,y\rangle|(x-a_1)^2+(y-b_1)^2 < r_1 \}\\
D_2 &= \{\langle x,y\rangle|(x-a_2)^2+(y-b_2)^2 < r_2 \}\\
\end{aligned}
$$
Now take some point $\langle u,v\rangle\in D_1$. Define a new set 
$$
D_{\langle u,v\rangle} = \{\langle x, y\rangle|\langle x,y\rangle\in D_1 \land (x-u)^2+(y-v)^2 < r_s^2(u,v) \}
$$
where $r_s(u,v)$ is some function that depends on $\langle u,v\rangle$.

The main idea is to define a disc $D_{\langle x,y\rangle}$ to always be $D_{\langle x, y\rangle}\subset D_1$ for all $\langle u,v\rangle\in D_1$. This means as $\langle u,v\rangle$ reaches the boundary of $D_1$, $r_s(u,v)\rightarrow 0$. So we set 
$$
r_s(u,v) = \frac{r_1-\sqrt{(u-a_1)^2+(v-b_1)^2}}{8}.
$$

Now we check if such a $D_{\langle u,v\rangle}$ satifies the conditions. Base case $u = a_1$ and $v=b_1$. Then $D_{\langle a_1,b_1\rangle}$  is in the circle. Then take 
$$
\lim_{\sqrt{(u-a_1)^2+(v-b_1)^2}\rightarrow r_1}r_s(u,v) = 0.
$$
So $D_{\langle u,v\rangle}\subset D_1$ for all $\langle u,v\rangle\in D_1$. 


Now suppose we look at $D_1$ and $D_2$ and assume $D_1 \cap D_2 \neq \emptyset$. We want to show that there always exists a disc $D_{\langle a,b\rangle}\subset D_1\cap D_2$ where $\langle a,b\rangle\in D_1\cap D_2$. Define two new sets 
$$
\begin{aligned}
D_{1\langle a,b\rangle}&=\{\langle x, y\rangle|\langle x,y\rangle\in D_1 \land (x-a)^2+(y-b)^2 < r_{1s}^2(u,v) \}\\
D_{2\langle a,b\rangle}&=\{\langle x, y\rangle|\langle x,y\rangle\in D_2 \land (x-a)^2+(y-b)^2 < r_{2s}^2(u,v) \}\\
\end{aligned}
$$
where $\langle a,b\rangle\in D_1\cap D_2$. We know $D_{1\langle a,b\rangle}\subset D_1$ for all $\langle a,b\rangle\in D_1$ and  $D_{2\langle a,b\rangle}\subset D_2$ for all $\langle a,b\rangle\in D_2$. Then for $D_1\cap D_2$ take disc that has $\text{min}\{r_{1s},r_{2s}\}$.


***(ii)*** Take $\langle a, b\rangle\in D_1\cap D_2$ then $\langle a, b\rangle\in D_{\langle a, b\rangle}$ by definiton.  
$$
\langle a, b\rangle\in \bigcup_{\langle u, v\rangle\in D_1\cap D_2}D_{\langle a, b\rangle}.
$$
Therefore $D_1\cap D_2\subseteq \bigcup_{\langle a, b\rangle\in D_1\cap D_2} D_{\langle a, b\rangle}$. 

Now take  

$$
\langle u, v\rangle\in\bigcup_{\langle a, b\rangle\in D_1\cap D_2} D_{\langle a, b\rangle}.
$$
Then  we know that  $\langle u,v\rangle\in D_{\langle u,v\rangle}\subset D_1\cap D_2$. Therefore   $D_1\cap D_2\supseteq \bigcup_{\langle a, b\rangle\in D_1\cap D_2} D_{\langle a, b\rangle}$. 

***(iii)*** To show that the collection of all open discs in $\mathbb{R}^2$ is a basis for a topology we show that 
$$
\mathbb{R}^2=\bigcup_{\langle a,b\rangle\in\mathbb{R}^2}D_{\langle a, b\rangle}.
$$

Take any $\langle x, y\rangle\in\mathbb{R}^2$. THen by definition $\langle x, y\rangle\in D_{\langle x, y\rangle}$. So 
$$
\langle x, y\rangle\in \bigcup_{\langle a, b\rangle\in\mathbb{R}^2}D_{\langle a, b\rangle}.
$$
Now take any 
$$
\langle x, y\rangle\in \bigcup_{\langle a, b\rangle\in\mathbb{R}^2}D_{\langle a, b\rangle}.
$$
Then $\langle x, y\rangle\in D_{\langle x, y\rangle}\subset\mathbb{R}^2$.

![[Exercise223.png]]
*Proof:* Take any open set $S\in\tau$. Then by [[Proposition for Euclidean topology on real numbers|proposition for euclidean topology on real numbers]] $S$ is a union of open intervals. Let 
$$
S = \bigcup_{x\in S}I_x
$$
where $I_x$ are open intervals that contain $x$. Take any open interval $I_x = (a_x,b_x)$ where $a_x<b_x$ and $a_x, b_x$ are real. Now any real number can be written as a sequence of rational e.g. $a_{ix}\rightarrow a_x$ and $b_{ix}\rightarrow b_x$. Then 
$$I_x = (a_x,b_x) = \bigcup_{i = 1}^{\infty}(a_{ix},b_{ix}).$$
Therefore
$$
S = \bigcup_{x\in S} I_x = \bigcup_{x\in S}\bigcup_{i=1}^\infty(a_{ix},b_{ix}).
$$
So any open set can be written as a union of members of $\mathcal{B}$.



![[Exercise224.png]]
**(i)** We know by [[The set of all rational numbers is countably infinite]] that $\mathbb{Q}$ is [[Countable, uncountable|countable]]. Now the basis in the previous exercise is defined as

$$
\mathcal{B}=\{(a,b)|a,b\in\mathbb{Q}\}.
$$
Clearly $\mathcal{B}$ is [[Equipotent|equipotent]] to $\mathbb{Q}\times\mathbb{Q}$. By [[Product of countably infinite sets|product of countably infinite sets]]  $\mathbb{Q}\times\mathbb{Q}$ is countable. Therefore by [[Equipotent and countable|equipotent and countable]] $\mathcal{B}$ is contable. Therefore the euclidean topology in $\mathbb{R}$ is second countable.

**(ii)** Let $X$ be an uncountable set. Let $(X,\tau)$ be a discrete space. Now for a $\mathcal{B}$ to be a basis for $\tau$, must contain atleast all the singleton sets of $X$. If we define 
$$
\mathcal{B} = \{\{x\}|x\in X\}.
$$
Then we know that this is the smallest basis we can have. Any other basis $\mathcal{B}$ must contain members of $\mathcal{B}$ and union of members of $\mathcal{B}$.

**(iii)** Let's prove that 
$$
\mathcal{B} = \{\langle a,b\rangle|\langle a,b\rangle\in\mathbb{Q}\times\mathbb{Q}\}
$$
where $a$ and $b$ come from open intervals e.g. $a\in(u_1,v_1)$ and $b\in (u_2,v_2)$. #ToBeProven 

**(iv)**  We know that all closed sets in a [[Finite Closed topology|finite closed topology]] are finite. If we show that there are countably many finite sequences of integers then we are done. 

![[Exercise226.png]]
We have defined the product topology here. #ToBeProven.

![[Exercise227.png]]
