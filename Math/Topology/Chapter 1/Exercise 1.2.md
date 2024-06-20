![[Exercise121.png]]
We have set $X = \{a,b,c,d,e,f\}$ and topology $\tau_1 = \{X,\emptyset,\{a\},\{c,d\},\{a,c,d\},\{b,c,d,e,f\}\}$. Since we are too lazy to list out all the subsets of $X$ we will first find all the [[Open and Closed sets|open sets]]. Then look at whether any of the open sets are [[Open and Closed sets|closed sets]]. In $\tau_1$ the following sets are open sets: $\{a\}$, $\{c,d\}$, $\{a,c,d\}$ and $\{b,c,d,e,f\}$. To check if there sets are closed sets we look at their complements: $\{b,c,d,e,f\}$, $\{a,b,e,f\}$, $\{b,e,f\}$ and $\{a\}$. We see that out of all the open sets only $\{a\}$ and $\{b,c,d,e,f\}$ are closed sets. The remaining subsets are neigther open or closed sets.

![[Exercise122.png]]
*Proof* If we can show that for every $x\in X$ there is $\{x\}\in\tau$ then we are done by [[Proposition with singleton sets]]. We start constructing set $A = X\backslash \{x\}$ where $x\in X$. Since $A\subset X$ it is a [[Open and Closed sets|closed set]]. By definiton of [[Open and Closed sets|closed sets]] $X\backslash A$ is an [[Open and Closed sets|open set]]. But $X\backslash A = X\backslash (X\backslash \{x\}) = \{x\}$. We have shown that $\{x\}$ is an open set. Since $x$ was arbitrarily chosen this is true for every element in $X$. By [[Proposition with singleton sets]] $\tau$ is a [[Discrete and indiscrete topology|discrete topology]].

![[Exercise123.png]]
We can choose $\tau = \{X,\emptyset,\{a\},\{b,c,d\}\}$. It is we wonder if having even number of sets in $\tau$ can always give a all clopen.
![[Exercise124.png]]
*Proof:* We need to show that for every $x\in X$ there is a $\{x\}\in \tau$. Then by [[Proposition with singleton sets]] we are done. We can construct set $A = X\backslash \{x\}$. Since $A\subset X$ it is infinite and therefore closed. This means that $X\backslash A$ is an open set. But $X\backslash A = \{x\}$. So we have shown that $\{x\}$ is an open set.
![[Exercise125.png]]
*Counter example:* We can take set $\mathbb{N}$ and make topology $\{\mathbb{N},\emptyset,\{1\}\}$. This is not an [[Discrete and indiscrete topology|indiscrete space]].

![[Exercise126.png]]
*Proof:* (i) all we need to show is that the three conditions cannot be satisfied properly. Looking at the proposition for [[Open and Closed sets|open sets]], we see that the union between open sets is an open set and the intersection between open sets is an open set. Therefore this means that $A\cup B\in\tau$ and $A\cap B\in\tau$. There are three cases. Case 1: $A\cup B = X$ then $A\cap B = \emptyset$. Case 2: $A\cup B = A$ then $A\cap B = B$. Case 3: $A\cup B = B$ then $A\cap B = A$. We see that the three given conditions cannot bet simultaneously satisfied. Only one condition can be satisfied.

(ii). We list the forms of possible topologies with exactly four sets. 
1. $\tau_1 = \{X,\emptyset\,\{1,2\},\{3,4\}\}$. There are  $4\choose 2$  ways to get this topology or 6 ways in total.
2. $\tau_2 = \{X,\emptyset\,\{1\},\{1,2\}\}$. There are $4\choose 2$ ways to get a doubleton set and $2\choose 1$ ways to get a singleton set. So there are 12 ways to get such a topology.
3. $\tau_3 = \{X,\emptyset\,\{1\},\{1,2,3\}\}$. There are $4\choose 3$ ways to get a tripleton set and $3\choose 1$ ways to get a singleton set. So there are 12 ways to get such a topology.
4. $\tau_4 = \{X,\emptyset\,\{1,2\},\{1,2,3\}\}$. There are $4\choose 3$ ways to get a tripleton set and $3\choose 2$ ways to get a doubleton set. So there are 12 ways to get such a topology. 

Therefore there are in total 6+12+12+12 = 42 ways to get topologies with exactly four sets in it.

![[Exercise 127.png]]
(i) *proof:* Suppose a set $X_n$ with $n$ elements has $M$ distinct topologies. We may list these topologies as $\tau_1,\tau_2,...,\tau_M$.  Now consider a set $X_{n+1}$ which has $n+1$ elements. Take any of the previously listed topologies and create set $\tau_i'=\tau_i\cup X_{n+1}$ for $i = 1,2,...,M$. If $\tau_i'$ is a topology then we have shown that $X_{n+1}$ has $M$ distinct topologies. Take an arbitrary element $S\in\tau_i'$ where $S\neq X_{n+1}$. Then we know for all elements of $\tau_i'$ other than $X_{n+1}$ the set $S$ satisfies the [[Axioms|axioms]]. We check if $S$ satisfies the axioms with $X_{n+1}$. First, $X_{n+1}\cup S=X_{n+1}\in\tau_i'$ and $X_{n+1}\cap S = S\in\tau_i'$. So we have shown that $\tau_i'$ are still topologies for $i = 1,2,...,M$. We know that the [[Discrete and indiscrete topology|indiscrete topology]] exists for every set i.e. $\tau = \{X_{n+1},\emptyset\}$. This means we have shown that there are atleast $M+1$ on $X_{n+1}$.