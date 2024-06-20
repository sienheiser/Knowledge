#GroupTheory 

Suppose we look at $S_5$. An element $g$ could be taking $1\rightarrow 4$, $2\rightarrow 1$, $3\rightarrow 5$, $4\rightarrow 2$ and $5 \rightarrow 3$. More compactly we could write $g = (142)(35)$ where $(142) = 1\rightarrow 4\rightarrow 2\rightarrow 1$ and $(35) = 3\rightarrow 5\rightarrow 3$. Notice how $(142)=(214)=(421)$. This means that we can move elements cyclically around and get the same answer. A cycle with $k$ elements is called a $k$-cycle.

Any permutation $P$ can be written as a product of cycles. Imagine we take an some integer between $1$ and $n$ and call it $a_1$. Then apply $P$ to $a_1$ giving $a_2$. Then $P$ to $a_2$ giving $a_3$; keep doing this until we reach back to $a_1$. Then we have formed a $j$-cycle $(a_1a_2a_3...a_j)$. Take another number $b_1$ which is not part of the $j$ cycle and repeate the process. We will see that $P = (a_1....a_j)(b_1..)..()$. 

Finally, if an element is can be written as $g = (13)(2)(4)(5)$, then we shorten it to $g = (13)$.