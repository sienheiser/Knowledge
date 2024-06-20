![[Exercise111.png]]
To solve this exercise we look at the [[Axioms|axioms]] to see whether the givens sets are a topology on $X$.

(a) This set satisfies the first axiom of $X$ and $\emptyset$ belonging being an element of $\tau_1$. The second axiom of the union of any number of elements from $\tau_1$ belonging to $\tau_1$ is satisfied. The third axiom is not satisfied since the intersection between $\{a,f\}\cap\{b,f\} = \{f\}\notin\tau_1$. Therefore $\tau_1$ is not a topology on $X$.

(b)  This set satisfies the first axiom of $X$ and $\emptyset$ belonging being an element of $\tau_2$. The second axiom of the union of any number of elements from $\tau_2$ belonging to $\tau_2$ is satisfied. The third axiom is not satisfied since the intersection between $\{a,b,f\}\cap\{a,b,d\} = \{a,b\}\notin \tau_2$. Therefore $\tau_2$ is not a topology on $X$.

(c)  This set satisfies the first axiom of $X$ and $\emptyset$ belonging being an element of $\tau_3$. The second axiom is not satisfied as $\{e,f\}\cup\{a,f\} = \{a,e,f\}\notin\tau_3$. Therefore $\tau_3$ is not a topology on $X$.

![[Exercise112.png]]
$\tau_1$ is not a topology on $X$ since $\{c\}\cup\{b\} = \{b,c\}\notin\tau_1$.  $\tau_2$ is not a topology on $X$ since $\{b,d,e\}\cap\{a,b,d\} = \{b,d\}\notin \tau_2$. $\tau_3$ is a topology on $X$ since it satisfies all the [[Axioms|axioms]].

![[Exercise113.png]]
I will only write the true statements. (a), (d), (g), (i), (l), (o).

![[Exercise114.png]]
*Proof:* Let $N$ be the numbers of sets $S_i\in\tau$ that we intersect. The base case is $N = 2$: $S_1\cap S_2\in\tau$ by the [[Axioms|axioms]]. Trial case $N=3$: 
$$S_1\cap S_2\cap S_3 \stackrel{1}{=}(S_1\cap S_2)\cap S_3\stackrel{2}{\in}\tau$$
where $\stackrel{1}{=}$ is true because the intersection operation is associative and $\stackrel{2}{\in}$ is true because we intersecting two sets that belong to $\tau$. If $N = 4$ then
$$S_1\cap S_2\cap S_3\cap S_4 \stackrel{3}{=}((S_1\cap S_2)\cap S_3)\cap S_4\stackrel{4}{\in}\tau$$
where $\stackrel{3}{=}$ is true because the intersection operation is associative and $\stackrel{4}{\in}$ is true because we intersecting two sets that belong to $\tau$. Suppose the intersection between $N = n-1$ sets belongs to $\tau$ then we look at $N = n$:

$$
S_1\cap S_2\cap ... \cap S_{n-1} \cap S_n \stackrel{5}{=}(...(S_1\cap S_2)\cap ... \cap S_{n-1})\cap S_n\stackrel{6}{\in}\tau
$$
where $\stackrel{5}{=}$ is true because associativity and $\stackrel{6}{\in}$ is true by definiton.

![[Exercise115.png]]

(i) The given topology satisfies the first axiom. Take the unions any sequence of intervals 
$$
\bigcup_i (-n_i,n_i) = \text{max}\{(-n_i,n_i)\}\in \tau_1.
$$
Finally taking sequence between any two open intervals gives
$$
(-n_i,n_i)\cap(-n_j,n_j) = \text{min}\{(-n_i,n_i),(-n_j,n_j)\}\in \tau_1
$$
So $\tau_1$ is a topology on $\mathbb{R}$.

(ii) $\tau_2$ is also a topology as the same arguments as above can be used.

![[Exercise116.png]]
*Proof*: We want to show $\tau_1$ (known as an **initial segment topology**) is a topology on $\mathbb{N}$. $\tau_1$ satisfies the first condition in the [[Axioms|axioms]]. Define sets $A_1 = \{1\}$, $A_2 = \{1,2\}$, $A_3 = \{1,2,3\}$,..... Then we know that all these sets $A_i\in\tau_1$. Now take any sequence of $A_i$ and take the union of them 
$$
\bigcup_{i\in I} A_i = A_{\text{max}\{I\}}\in\tau_1.
$$
So the second condition is satisfied in [[Axioms|axioms]]. Now we try to show that taking the third axiom is satisfied. Take any two sets $A_i$ and $A_j$. Then 
$$
A_i\cap A_j = A_{\text{min}\{i,j\}}\in\tau_1
$$
We have shown that $\tau_1$ is a topology on $\mathbb{N}$.

(ii)We want to show $\tau_2$ (known as an **final segment topology**) is a topology on $\mathbb{N}$. We see that it satisfies the first [[Axioms|axiom]]. Define sets $B_1 = \{n\}$, $B_2 = \{n,n+1\}$, $B_3 = \{n,n+1,n+2\}$, .... Now we look at the whether the union any number of these sets still belongs to $\tau_2$. We take
$$
\bigcup_{i\in I}B_i = B_{\text{max}\{I\}}\in\tau_2.
$$
So the second [[Axioms|axiom]] holds. Now we look the intersection between any two set

$$
B_i\cap B_j = B_{\text{min}\{i,j\}}\in\tau_2.
$$
We have shown that the third [[Axioms|axiom]] holds. Therefore, $\tau_2$ is a topology on $\mathbb{N}$.

![[Exercise117.png]]
(a) We have a [[Discrete and indiscrete topology|discrete topology]] and [[Discrete and indiscrete topology|indiscrete topology]]. Then we have topology of form $\tau = \{X,\emptyset,\{a\}\}$; there are two of these topologies. So in total we have four topologies for this case.

(b) We again have the [[Discrete and indiscrete topology|discrete topology]] and [[Discrete and indiscrete topology|indiscrete topology]]. We have three topologies of form $\tau = \{X,\emptyset,\{a\}\}$ because there are three ways to choose the singleton set. We have three topologies of form $\tau = \{X,\emptyset, \{a,b\}\}$ because there are three ways to choose the doublet set. We have nine topologies of form $\tau = \{X,\emptyset,\{a\},\{a,b\}\}$ because there are three ways to choose the singleton set and a doubleton set. Finally we have topology of form $\tau = \{X,\emptyset, \{a,b\},\{a,c\},\{a\}\}$. There are only three of these topologies because intersection between any two doubleton set is always a singleton sets in this case. So we can only have three types of intersections. Therefore there are 1+1+3+3+9+3 = 20 topologies on $X$.

![[Exercise118.png]]
*Proof:* We want to show that $\tau$ is a [[Discrete and indiscrete topology|discrete topology]]. We can do this by using the [[Proposition with singleton sets|proposition with singleton sets]]. All we have to do is show that for every $x\in X$, there is a singleton set $\{x\}\in\tau$. 

We start by constructing two subsets $A$ and $B$ of $X$, with properties $A\cap B=\emptyset$ and $A\cup B = X$. Since they are infinite subsets they belong to topology $\tau$. Now take an arbitrary element $a\in A$ and create set $B' = B\cup \{a\}$. By construction $B'\in \tau$ since it is an infinite subset of $X$. Furthermore, $A\cap B' = \{a\}\in \tau$ by [[Axioms|axiom 3]]. Since $a$ is arbitrary this is true for every element of $A$. We have shown that there exist singleton sets in the topology for each element of $A$. WLOG this is true every element of $B$. Therefore, we have shown that for any $x\in X$ there is $\{x\}\in\tau$. By [[Proposition with singleton sets|proposition with singleton sets]] $\tau$ is a [[Discrete and indiscrete topology|discrete topology]].

![[Exercise119.png]]
1. We can choose intervals $(a_1,b_1)$ and $(a_2,b_2)$ where $a_1 < b_1 < a_2 < b_2$. Then $$(a_1,b_1)\cup(a_2,b_2)\notin \tau_1$$. We  have shown that the union between any two sets in $\tau_1$ does not necessarily belong to $\tau_1$. So it is not a topology on $\mathbb{R}$.
2.  It clear that the given set $\tau_2$ satifies [[Axioms|axioms]] 1 and 3. It also satisfies axiom 2 for unions between finite amount of sets. Since we are looking at any real positive number. Any converging sequence of real positive numbers $r_n$ will converge to another real positive number. There for axiom 2 is satisfied and $\tau_2$ is a topology on $\mathbb{R}$.
3.  We are looking at a set that contains all open intervals of any positive rational numbers. If we take the infinite union of $$\bigcup_{n = 1}^\infty (-(1+\frac{1}{n})^n,(1+\frac{1}{n})^n) = (-e,e)\notin \tau_3$$ where $e$ is not a rational number. Therefore $\tau_3$ is not a topology on $\mathbb{R}$.
4.  Same reason as in above  $$\bigcup_{n = 1}^\infty [-(1+\frac{1}{n})^n,(1+\frac{1}{n})^n] = (-e,e)\notin \tau_4.$$ So $\tau_4$ is not a topology on $\mathbb{R}$.
5.  We can find a monotonically increase sequence of irrational numbers that converge to a rational number. The sequence is the following: $$(-\sqrt{2},\sqrt{2})\cup(-\sqrt{2}^\sqrt{2},\sqrt{2}^\sqrt{2})\cup (-\sqrt{2}^{\sqrt{2}^\sqrt{2}},\sqrt{2}^{\sqrt{2}^\sqrt{2}})\cup...=(-2,2)\notin\tau_5$$
6.  $\tau_6$ is not a topology on $\mathbb{R}$ for the same reason as above.
7.  We can take a monotonically increasing converging infinite sequence of real positive numbers $r_n$. Then $$\bigcup_{n}^\infty[-r_n,r_n) = (-r,r)\notin\tau_7.$$ So the second [[Axioms|axiom]] is not satisfied. Therefore $\tau_7$ is not a topology on $\mathbb{R}$.
8.  $\tau_8$ is not a topology on $\mathbb{R}$ for the same reason as $\tau_7$.
9.  If we take monotonically increasing positive converging sequence of real numbers $r_n$ then we can take the following union of intervals: $$\bigcup_{n =  1}^\infty [-r_n,r_n] = (-r,r)\stackrel{1}{\in}\tau_9$$ where $\stackrel{1}{\in}$ is true because of the defininton of $\tau_9$.
10.  Take any sequence of positive integers $n_i$ that is monotonically increasing, it is not possible for such a sequence to converge. Therefore $$\bigcup_{i = 1}^\infty [-n,n] = (-\infty,\infty)\in\tau_{10}.$$ We do not need to worry for intervals of real numbers $(-r,r)$ where $r$ is a positive real number because of $\tau_2$.
Therefore (ii), (ix) and (x) are topologies on $\mathbb{R}$.