Definitions: A monoid $m$ is a set that comes equipped with operation $*$ with the following properties
1. $\forall a,b\in m a*b\in m$
2. $\exists e\in m, \forall a\in m e*a=a*e$
3. Associative under the operation

## observation
The set of natural numbers with addition as operation is a monoid. We can get the following pattern
$$3=3+0 = 2+1 = 1 + 2 = 0+3=3$$
There is no reason that $2+1 = 3+0$ or $2+1 = 1+2$. That is just accidental. We can to construct monoid without this. This is called a free monoid.

## Using generators to construct free monoid
Suppose we start with the following set $\{e,a,b\}$ where $e$ is the identity and we have operation $*$. We can construct the following set
$$\{e,a,b,aa,bb,ab,ba\}$$
where $aa = a*a, ba = b*a$ etc. We can continue adding to set and getting
$$\{e,a,b,aa,bb,ab,ba,abb,aba,bab,baa,....\}$$
In this way we get a free monoid? Not sure about this. But anyway the set we get can be viewed as containing all possible lists of $a$ and $b$ e.g. $abba=[a,b,b,a]$  

## Constructing free monoid using categories only.

Lets define the category of monoids as $\text{Mon}$ to contain monoids as objects and homomorphism between two monoids as morphisms between them. Lets define the the category of sets as $\text{Set}$ to contain sets as objects and functions between two sets as morphisms between them.

Can we have a functor from $\text{Set}$ to $\text{Mon}$? No! I am not sure why so I will speculate. Since the category $\text{Set}$ is rich in morphisms between sets it may not be possible to inject the category into $\text{Mon}$. On the flip side we can have a functor $U:\text{Mon}\rightarrow \text{Set}$.
![[Monoid.jpg]]
In the above figure we see the two categories $\text{Mon}$ and $\text{Set}$. The basic pattern that we want to apply universal construction to is the relation between objects $(m,Um,X)$. So when we do universal construction we need a method of ranking different patterns. We say that $(m,Um,X)$ is better than $(n,Un,X)$ if there is a homomorphism from $m$ to $n$. The best $m$ (free monoid) is the one that has a unique homomorphism to any other monoid.

We obtain the following relations
1. $p\circ Uh = q$