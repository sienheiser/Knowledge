---
aliases: [consistent]
---

*Definition:* An [[Axiomatic system|axiomatic system]] is **consistent** if there exists a proposition $q$ which cannot be proven from the axioms.

*Idea behind the definitoin:* consider and axiomatic system containint contradicting propositions: 
$$
....,S,....,\neg S,...
$$
Then by (M) from [[Proof|proof]] we can make $S\land \neg S\implies q$ is a tautology becuase of definiton of $\implies$ from [[Logical operators|logical operators]]. 

*Theorem:* Propositional logic is consisten.
*Proof:* Show that there exits a proposition that cannot be proven within propositional logic. Propositional logic has an empty sequence of axioms. Only (T) and (M) are valid from [[Proof]|proof]. Clearly any tautalogy can be proven. This means that $q\land \neg q$ cannot be proven.

*Remark:* It is difficult to check whether any axiomatic system is consistent.