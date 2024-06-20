*Def/Theorem:* The smallest $\sigma$-algebra denoted $\sigma(E)$ for a set $M$ that contains (among, other subsets of $M$) a collection of subsets $E\subseteq P(M)$ is called/def as
$$
\begin{aligned}
\sigma(E)&:= \{A\subseteq M|\forall \sigma-\text{algebras  }\sigma\text{ of  } M\text{ with  } E\subseteq \sigma|A\in\sigma\}\\
& = \bigcap_{E\subseteq\sigma}\sigma
\end{aligned}
$$

Lets understand the elements of the above set. We have a set $E$ that contains other sets subsets of $M$. Now set $M$ can have many different $\sigma$-algebras. We only consider those $\sigma$-algebras that contain $E$ or are $E$. Then $\sigma(E)$ consists of all elements the sigma algebra that contain or are $E$.

I do not think $E$ needs to be a sigma algebra on $M$.


*Theorem:* Every $\sigma$-algebra can be written as $\sigma = \sigma(E)$ for some $E$.

