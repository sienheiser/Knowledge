*Proposition:* Let $(X,\tau)$ and $(Y,\tau_1)$  be [[Axioms|topological spaces]] and $f:(X,\tau)\rightarrow(Y,\tau_1)$ surjective and [[Continuous functions|continuous]]. If $(X,\tau)$ is connected, then $(Y,\tau_1)$ is connected. 

*Proof:* Suppose that $(Y,\tau_1)$ is connected. Then it has a proper non empty clopen subset $S$. Meaning $S\neq Y$ or $S\neq \emptyset$. Look at $f^{-1}(S)$, since $f$ is [[Injective, Surjective and Bijective|surjective]] then for each $y\in Y$ there exists $x\in X$ such that $f(x)=y$. Therefore $f^{-1}(S)\neq\emptyset$. Furthermore more we know that only $f^{-1}(Y)=X$ because $f$ is surjective. Since $S\neq Y$ then $f^{-1}(S)\neq X$. Because $f$ is continuous and by proposition [[Continous maps and closed sets]]  $f^{-1}(S)$ is also a clopen set of $(X,\tau)$ therefore $(X,\tau)$ is not connected, which is a contradiction.
