### Axiom
$x\in y$ is a [[Propositional logic|proposition]] if and only if $x$ and $y$ are both sets.

$$
\forall x:\forall y:(x\in y)\lxor \neg(x\in y)
$$
where $\lxor$ is the exlusive or. The statement says for $x$ and for all $y$ either $x$ element $y$ or $x$ not element $y$.


### Counter example (Russel paradox)
Assume there is some $u$ that contains all sets that do not contain as an element themselves. To be precise
$$
\exists u:\forall z:(z\in u\iff z\notin z).
$$
Question: Is $u$ a set? If $u$ was a set then one must be able to decide whether $u\in u$ is true or false.
Assume $u\in u$ is true then by definiton of $u$, $u\notin u$. This is a contradiction. After that assume that $u\in u$ is false. This is true if and only if $u\notin u$, then by definiton of $u$, $u\in u$. We get another contradction. 
Conclusion: $u$ is not a set.

