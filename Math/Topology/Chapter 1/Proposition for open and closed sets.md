*Proposition:* If ($X,\tau$) is any topological space, then
1. $X$ and $\emptyset$ are open sets,
2. the union of any number of open sets  (finte or infinite) is an open set,
3. the intersection of a finite number of open sets is an open set.

*Proof:* The first statement and second statement is by definiton of [[Open and Closed sets|open sets]] and the [[Axioms]]. The third statement is by definiton of [[Open and Closed sets|open sets]] and result from Exercise 1.1.4.

*Proposition:* If ($X,\tau$) is any topological space, then
1. $X$ and $\emptyset$ are closed sets,
2. the intersection of any number closed sets (finite or infinite) is a closed set
3. the union of a finite number of closed sets is a closed set.

*Proof:* The first statement is by definiton of [[Open and Closed sets|closed sets]] and [[Axioms]]. For the third statement we want to show that $S_1\cup S_2\cup S_3\cup...\cup S_n$ is a closed set where $S_i$ are subsets of $X$. We do this by showing that $X\backslash S_1\cup S_2\cup S_3\cup...\cup S_n$ is an open set. We know that $X\backslash S_i$ is an open set. We have identity 
$$
X\backslash S_1\cup S_2\cup S_3\cup...\cup S_n = X\backslash S_1\cap X\backslash S_2 \cap X\backslash S_3\cap ... \cap X\backslash S_n.
$$
On the right hand side we have a finite intersection of open sets which is also an open set. Therefore the finite union of all closed sets is a closed set.

We prove the second statement. We want to show that the infinite intersection of closed sets is a closed sets. There we want to show that $X\backslash S_1\cap S_2\cap S_3\cap ...$ is open. We have the following identity
$$
X\backslash  S_1\cap S_2\cap S_3\cap ... = X\backslash S_1\cup X\backslash S_2\cup X\backslash S_3\cup ....
$$
The righthand side is an infinite union of open sets. Therefore the lefthand side is an open set. Which results in the infinite intersection of closed being a closed set. We note it is possible that is proof is only true for countably infinite sets.
