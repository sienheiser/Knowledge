*Proposition:* The union of any [[Countable, uncountable|countable]] family of countable sets is a countable set.

*Proof:* There are four cases we need to prove. 

Case 1:
Union of [[Countable, uncountable|countably infinite]] family of countably infinite sets is countable by lemma [[Countably infinite family of countably infinite sets]]. 

Case 2: Finite family of countable infinite sets. This means we have sets $S_1, S_2,...,S_n$ for some $n\in \mathbb{N}$. Since each $S_i$ is countably infinite $S_i=\{s_{i1},s_{i2},...\}$. Place $s_{ij}$ in the $i$th row and $j$th column of an array. This array has finite number of rows because there are finite number of sets. We can make a list of all the elements of the array by starting at $s_{11}$ and going to element $s_{n1}$ (going down the column). Then shift to the next column on the right and go up the column. In this manner all the elements of the array are listted. Therefore this is a countable set.

Case 3: Countably infinite family of finite sets. This means we have $S_1, S_2,...$ where each $S_i$ is finite. Make an array like in the previous case. This array has an infinite number of rows and finite number of columns. We may list all the elements of this array by the following algorithm
1. Start at $s_{11}$.
2. Move to right until reaching the last column
3. Move one row down
4. Move to the left until reaching the first column
5. Move one row down
6. Repeat from step 2.

Since we have  a list the union of countably infinite family of finite sets is countable.

Case 4: Finite family of finite sets. This is trivially countable.

