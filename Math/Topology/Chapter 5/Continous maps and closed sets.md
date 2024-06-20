*Proposition:*  Let $(X,\tau)$ and $(Y,\tau')$ be topological spaces. Then $f:X\rightarrow Y$ is continous if and only if for every closed subset $S$ of $Y$, $f^{-1}(S)$ is a closed subset $X$.

*Proof:* Let $f$ be continous and let $S$ be closed subet of $Y$. Then $Y\backslash S$ is an open subset $Y$. Therefore $f^{-1}(Y\backslash S)\in\tau$. But 
$$
f^{-1}(Y\backslash S)=X\backslash f^{-1}(S),
$$
because 
$$
\begin{aligned}
f^{-1}(Y\backslash S)&=\{x|f(x)\in Y\land f(x)\notin S\}\\
X\backslash f^{-1}(S)&=\{x|x\in X\land x\notin f^{-1}(S)\}
\end{aligned}
$$
Therefore $x\in X\backslash f^{-1}(S)\iff x\in X\land x\notin f^{-1}(S)\iff f(x)\in f(X)\land f(x)\notin f(f^{-1}(S))\iff f(x)\in Y\land f(x)\notin S$. So we see that $X\backslash f^{-1}(S)$ is still an open set. 

