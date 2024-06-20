### Axiom
There exists a set that contains no elements. In logic this becomes 
$$
\exists x:\forall y:y\notin x.
$$

*Theorem:* There is only one empty set. We call it $\emptyset$.
*Proof:* Assume $x$ and $x'$ are both empty sets. But then 
$$
\forall y:(y\in x)\implies (y\in x').
$$
The above statement is arbitrarily true. This is because $y\in x$ is always false, but by definiton of $\implies$ from [[Logical operators|logical operators]] having another false proposition $(y\in x')$ makes $(y\in x)\implies (y\in x')$ always true. Therefore $x\subseteq x'$.

Conversely
$$
\forall y:(y\in x')\implies (y\in x).
$$
Therefore, $x'\subseteq x$.