### Axiom 
Let $x$ and $y$ be sets. Then there exists a set, $u$, that has as its elements precisely the sets $x$ and $y$.

$$
\forall x:\forall y:\exists u:\forall m:(m\in u\iff m=x\lor m=y).
$$
The logical statement reads: for all $x$, for all $y$, there exists $u$ such that for all $m$, such that $m$ element $u$ if and only if $m=x$ or $m=y$.


We give notation 
$$
u = \{x,y\}.
$$
There could be a problem that $\{x,y\}\neq\{y,x\}$. We can show that both are the same by showing they are a subset of each other. Take any $a\in\{x,y\}$. Then $a=x\lor y$. This means $a\in\{x,y\}$. So $\{x,y\}\subseteq\{y,x\}$. The converse can be shown in the same way.  

If $x$ and $y$ are the same sets then 
$$
\{x,x\} = \{x\}.
$$
Because two same sets does not add any extra information.


