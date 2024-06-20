![[Exercise131.png]]

(a) *Proof:* Let $A = f^{-1}(\bigcup_{j\in J}B_j)$ and $A_j = f^{-1}(B_j)$. Then we want to show that $A = \bigcup_{j\in J}A_j$. We do this by taking any element $x\in A$ and showning that $x\in\bigcup_{j\in J}A_j$ and taking any element $x\in \bigcup_{j\in J}A_j$ and show that $x\in A$. 

We take any $x\in A$ then by definiton of [[Inverse Image|inverse image]] we have that $f(x)\in \bigcup_{j\in J}B_j$. This means at least one of the $B_j$ must contain $f(x)$. Let $f(x)\in B_i$. Then by definiton $x\in\bigcup_{j\in J}A_j$ since $x\in A_i=f^{-1}(B_i)$. So we have shown $A\subseteq \bigcup_{j\in J}A_j$.

Now take any $x\in\bigcup_{j\in J}A_j$. Then by $x$ belongs to atleast one of the $A_j$. Let $x\in A_i$. By definiton of [[Inverse Image|inverse image]] $f(x)\in B_{j}$. This means that $f(x)\in\bigcup_{j\in J}B_j$. By definiton of [[Inverse Image]] $x\in A=f^{-1}(\bigcup_{j\in J}B_j)$.

(b) *Proof:* We define $A=f^{-1}(\bigcap_{j=1}^{n}B_j)$ and $A_j= f^{-1}(B_j)$. We want to show $A=\bigcap_{j=1}^{n} A_j$. We do this by showing if $x\in A$ then $x\in\bigcap_{j=1}^{n}A_j$ and if $x\in\bigcap_{j=1}^{n}A_j$ then $x\in A$.

Start by taking $x\in A$. Then by definiton of [[Inverse Image|inverse image]] $f(x)\in\bigcap_{j=1}^{n}B_j$. This means $f(x)\in B_j$ for $j=1,2,3,...,n$ . Then by definiton of inverse image $x\in A_j$ for $j=1,2,3,...,n$. Therefore $x\in\bigcap_{j=1}^{n}A_j$. We have shown $A\subseteq \bigcap_{j=1}^{n}A_j$.

Now take $x\in\bigcap_{j=1}^{n}A_j$. This means $x\in A_j$ for $j=1,2,3,...,n$. Then by definiton of [[Inverse Image|inverse image]] $f(x)\in B_j$ for $j=1,2,3,...,n$. Therefore $f(x)\in\bigcap_{j=1}^{n}B_j$. Then by definiton of inverse image $x\in A=f^{-1}(\bigcap_{j=1}^{n}B_j)$. We have shown that $\bigcap_{j=1}^{n}A_j\subseteq A$. Therefore $A=\bigcap_{j=1}^{n}A_j$.

(c) *Proof:* We define the sets $X = Y = \mathbb{N}$ and  the function $f:X\rightarrow Y$ as $f(1)=f(2)=1$, $f(3)=f(4)=2$, $f(5)=f(6)=3$ and so on. Take $A_1 = \{1,2,4\}$ and $A_2 = \{2,3\}$. Then $f(A_1\cap A_2)=f(\{2\})=1$ and $f(A_1)\cap f(A_2)=\{1,2\}\cap\{1,2\}=\{1,2\}$. Therefore $f(A_1\cap A_2)\neq f(A_1)\cap f(A_2)$.

![[Exercise132.png]]
According to the [[Finite Closed topology|definiton]], all [[Open and Closed sets|closed sets]] in a finite closed topology must be finite. The topology $\tau_1$ consists of $\mathbb{N},\emptyset$ and every set $\{1,2,3,...,n\}$. Clearly $\mathbb{N}\backslash\{1,2,3,...,n\}$ is an infinite set therefore it is not closed in a finite closed topology.  Therefore, $\tau_1$ is not a cofinite topology.

The topology $\tau_2$ consists of $\mathbb{N},\emptyset$ and every set $\{n,n+1,n+2,...\}$. Clearly $\mathbb{N}\backslash\{n,n+1,n+2,...\}$ is finite. But set $\mathbb{N}\backslash \{2\}\notin \tau$. Therefore $\tau$ is not a cofinite topology.

![[Exercise133.png]]
In the question T$_1$ spaces (T one space) have been defined. 
1. We have shown in [[Exercise 1.2|exercise122]] that every subset of $X$ in a [[Discrete and indiscrete topology|discrete space]] $(X,\tau)$ is a [[Open and Closed sets|closed set]]. Therefore all the singleton sets are closed. Therefore, discrete spaces are $\text{T}_1$-spaces. 
2. An [[Discrete and indiscrete topology|indiscrete space]] $(X,\tau)$ with at least two points is not a $\text{T}_1$-space since for example $X = \{a,b\}$ then $X\backslash\{a\}=\{b\}\notin \tau$.
3. For a [[Finite Closed topology|cofinite topology]] all finite sets are closed by definiton. Therefore it is a $\text{T}_1$ space.
4. Here $X = \{a,b,c,d,e,f\}$ and $\tau = \{X,\emptyset,\{a\},\{c,d\}, \{a,c,d\},\{b,c,d,e,f\}\}$. Clearly not every singleton set is closed. Therefore $(X,\tau)$ is not a $\text{T}_1$-space.
5. $\tau$ consists of $\mathbb{R},\emptyset$ and every interval $(-n,n)$ where $n$ is a positive integer. We look whether singleton set $\{0\}$ is closed. This means $\mathbb{R}\backslash\{0\}$ should be open, but this is not the case with the defined $\tau$. Therefore $(\mathbb{R},\tau)$ is not a $\text{T}_1$-space.
6.  $\tau$ consists of $\mathbb{R},\emptyset$ and every interval $[-n,n]$ where $n$ is a positive integer. This is not a $\text{T}_1-$space for the same reason as in 5.
7.  $\tau$ consists of $\mathbb{R},\emptyset$ and every interval $[-n,\infty)$ where $n$ is a positive integer. This is not a $\text{T}_1-$space for the same reason as in 5 and 6.
8.  $\tau$ consists of $\mathbb{N},\emptyset$ and every set $\{1,2,3,...,n\}$ where $n$ is a positive integer. Clearly set $\mathbb{N}\backslash \{1\}$ is not an open set. Therefore, $(\mathbb{N},\tau)$ is not a $\text{T}_1$-space.
9.  $\tau$ consists of $\mathbb{N},\emptyset$ and every set $\{n,n+1,n+2,...\}$ where $n$ is a positive integer. Clearly $\mathbb{N}\backslash \{2\}\notin\tau$. Therefore this is not a $\text{T}_1$-space.

![[Exercise134.png]]
*Proof:* We are given $\tau$ which is a [[Finite Closed topology|cofinite topology]] on a set $X$. If $\tau$ is a [[Discrete and indiscrete topology|discrete topology]] on $X$ we want to show that $X$ can only be a finite set. Since $\tau$ is a cofinite topology on $X$ we know every finite subset of $X$ is a [[Open and Closed sets|closed set]]. If $\tau$ is also a discrete topology on $X$ we know that every subset of $X$ is a closed set. Therefore if $X$ was an infinite then we would have infinite closed sets which is a contradiction to the assumption that $\tau$ is a cofinite topology. Therefore $X$ is a finite set.

![[Exercise135.png]]
1. *Proof:* $\text{T}_1$-spaces have every singleton set of $X$ as a [[Open and Closed sets|closed set]]. All we have to do is take any two distinct points $a,b\in X$ and show that in a $\text{T}_1$-space either there exists an [[Open and Closed sets|open set]] that contains $a$ and not $b$, or there exists an open set that contains $b$ but not $a$. 
Take two distinct points $a,b\in X$. Because $(X,\tau)$ is a $\text{T}_1$-space we know that $\{a\}$ and $\{b\}$ are closed sets. Therefore in $\tau$ there exists sets that contain $a$ but not $b$ or sets that contain $b$ but not $a$.

2. (i) is a discrete space which is a $\text{T}_1-$space. Therefore is it also a $\text{T}_{0}-$ space. (ii) is an indiscrete space therefore it is not a $\text{T}_{0}-$space since $X,\emptyset$ do no satisfy the conditions. (iii) For a [[Finite Closed topology|cofinite topology]] every finite set is closed. Therefore the singleton sets are closed. This means that we take any two distinct point $a,b\in X$ then sets $X\backslash\{a\}$ and $X\backslash \{b\}$ are opensets therefore cofinite topologies are $\text{T}_0-$spaces. (iv) is not a $\text{T}_0$-space because taking points $b,c\in X$. We see in the topology that $b$ only appears in set $\{b,c,d,e,f\}$. But $c$ also appears here. 
3. We can make topolgies $\{X,\emptyset,\{a\}\}$ and $\{X,\emptyset,\{b\}\}$. These topolgies on $X$ do not give $\text{T}_1-$spaces because not all singleton sets are closed sets. But they satisfy at least one of the conditions to be $\text{T}_0-$space.
4. We know that the initial segment topology (defined in [[Exercise 1.1|exercise 1.1.6]]) contains $\mathbb{N},\emptyset$ and  every set of form $\{1,2,...,n\}$ where $n$ is a positive integer. Take two distinct points $x_1,x_2\in \mathbb{N}$. WLOG if $x_1 < x_2$ then we know set $\{1,2,...,x_1\}\in\tau$. Therefore $(\mathbb{N},\tau)$ is a $\text{T}_0-$space. Now we look at the final segment topology (defined in [[Exercise 1.1|exercise1.1.6]]). It contains $\mathbb{N},\emptyset$ and every set $\{n,n+1,...\}$. Take two disctinct points $x_1,x_2\in \mathbb{N}$. WLOG if $x_1 < x_2$ then we know set $\{x_2,x_2+1,...\}\in\tau$. Therefore $(\mathbb{N},\tau)$ is a $\text{T}_0-$space.

![[Exercise136.png]]
#NotProvenYet


![[Exercise137.png]]
1. Let $X = \{a,b,c\}$. Then define topologies $\tau_1 = \{X,\emptyset,\{a\}\}$ and $\tau_2 = \{X,\emptyset,\{b\}\}$ on $X$. Then take $\tau_1\cup\tau_2=\{X,\emptyset,\{a\}\{b\}\}$ which is not a topology on $X$ because $\{a,b\}\notin \tau_1\cup\tau_2$.
2. To show  $\tau_4$ is a topology on $X$ we start by noting that all members of $\tau_4$ must belong to $\tau_1$ and $\tau_2$. Since $\tau_1$ and $\tau_2$ are topologies the common memebers among the topologies should satisfy the [[Axioms|axioms]]. Let us denote these common memebers as $S_i$ where $i\in I$ and $I$ is an index set. Then we know in $\tau_1$ and $\tau_2$ that $$\bigcup_{i\in I} S_i\in\tau_1,\tau_2$$ and $$S_i\cap S_j\in\tau_1\tau_2$$ for any $i,j\in I$. Since these same members belong to $\tau_4$ they also satisfy axioms 2 and 3. Finally since $\tau_1$ and $\tau_2$ are topologies $X,\emptyset\in \tau_1,\tau_2$ therefore $X,\emptyset\in\tau_4$. Therefore $\tau_4$ is a topology on $X$.

3. Since $(X,\tau_1)$ and $(X,\tau_2)$ are $\text{T}_1-$spaces we know that all the singleton sets of $X$ are closed sets of $\tau_1$ and $\tau_2$. Take any $x\in X$ then we know $\{x\}$ is a closed set. Therefore $X\backslash \{x\}\in\tau_1,\tau_2$. This means that $X\backslash \{x\}\in\tau_4$. Therefore, we have shown that all singleton sets are still closed in $\tau_4$.

4. Let $X=\{a,b\}$. Then define topologies $\tau_1=\{X,\emptyset,\{a\}\}$ and $\tau_2=\{X,\emptyset,\{b\}\}$. Then $\tau_4 = \tau_1\cap\tau_2=\{X,\emptyset\}$. $\tau_4$ is not a $\text{T}_0-$space.

5. Let the intersection between $n$ topologies be a topolgy. Base case $n=2$. We have proven in $(2)$ that the intersection between two topologies is a topology. Assume that the intersection between $n-1$ topolgies is still a topology on $X$. Then $$\bigcap_{i=1}^{n}\tau_i=\tau_n\cap\bigcap_{i=1}^{n-1}\tau_i\stackrel{1}{=}\tau_n\cap\tau'\stackrel{2}{=}\tau$$ where $\stackrel{1}{=}$ is true because of the induction hypothesis and $\stackrel{2}{=}$ is true because the intersection between two topologies is still a topolgy.
6. #NotProvenYet 