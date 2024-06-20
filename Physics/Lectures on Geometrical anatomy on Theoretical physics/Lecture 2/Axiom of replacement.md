### Axiom
Let $R$ be a funcitonal relation. Let $m$ be a set. Then the image of $m$ under $R$ is again a set.

$$\forall m:(\forall x\in m\exists!y:R(x,y)\implies\exists B:\forall y:[y\in B\iff \exists x\in m:R(x,y)]).$$
The intuition of this axiom is that if you some set, x some map $R$ such that $R:x\rightarrow y$. Then $y$ is a set.

### Principle of restricted comprehension (PCR)

The axiom of replacement implies, but is not implied by, the principle of restricted comprehension: Let $P$ be a predicate of one variable and let $m$ be a set. Then those elements $y\in m$ for which $P(y)$ holds constitute a set. 

Notation: $\{y\in m|P(y)\}$.

*Proof:* Case 1: $\neg\exists y\in m: P(y)$ in this case $\{y\in m| p(y)\}:=\emptyset$.
Case 2: $\exists \hat{y}\in m: P(\hat{y})$. Define $R(x,y):= (P(x)\land x=y)\lor (\neg P(x)\land \hat{y}=y)$. Claim $R(x,y)$ is a functional. It seems to satisfy the definiton of a functional. We may define the image as $\text{im}_R(m) := \{y\in m| P(y)\}$.

##### Complement
Let $u\subseteq m$. Then $m\backslash u:=\{x\in m|x\notin u\}$ is a set due to PCR, ultimately due to axiom of replacement.


##### Intersection
Let $x$ be a set. Define $$\bigcap x = \{a\in u\land a\in m|(u\in x\land m\in x)\land u\neq m\}.$$



