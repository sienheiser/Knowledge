#GroupTheory 
Let a group $G$ with $n$ elemnts have a [[Subgroups|subgroup]] $H$ with $m$ elements. Then $m$ is a factor of $n$. That is to say $n/m$ is an integer.

Proof: Suppose $H$ is a subgroup of $G$ with $m$ elements $\{h_1,h_2,...,h_m\}$. Suppose we take an element $g_1$ from $G$. Then we create set $\{h_1g_1,h_2g_1,...,h_mg_1\}$ which we denote as $\{h_1,h_2,...,h_m\}g_1$. The created set is not a group because it does not have an identity element. 

Claim 1: All the elements in the new set are different. Proof by contradiction: Suppose there is $h_a$ and $h_b$ such that $g_1h_a = g_1h_b \implies h_a = h_b$ which is a contradiction. So all elements in the set are different. 

Claim 2: None of the elements in the created set belong to $H$. Proof by contradiction: Suppose there is $h_a$ and $h_b$ such that $g_1 h_a = h_b \implies g_1 = h_a^{-1}h_b$ which is a contradiction.

Now take another element $g_2$ which does not belong to the group $H$ and $\{h_1,h_2,...,h_m\}g_1$ and create $\{h_1,h_2,...,h_m\}g_2$. The elements in set $\{h_1,h_2,...,h_m\}g_2$ satisfy claim 1 and claim 2. 

Claim 3: None of the elements in $\{h_1,h_2,...,h_m\}g_2$ belong to $\{h_1,h_2,...,h_m\}g_1$. Proof by contradiction: Suppose there is an $h_a$ and $h_b$ such that $h_a g_1 = h_b g_2\implies g_2 = h_b^{-1}h_ag_1 = h_c g_1$ which is a contradiciton.

Then we can keep doing the same process with elements that do not belong to the previous sets. If there are $k$ such elements then we have created $k$ sets with $m$ elements in each set. Therefore $n = mk$. 

#### Consequences

We define the group $Z_n$ where $n$ is an integer as the $1/n$  roots of 1. Example square roots of 1 is $Z_2 = \{1,-1\}$, $Z_3 = \{1, \exp(\frac{2\pi i }{3}),\exp(\frac{4\pi i}{3})\}$. We can see that the $Z_3$ is a subgroup of $Z_{12}$ but not $Z_{14}$. If $p$ is a prime number then $Z_p$ does not have nontrivial subgroups. 