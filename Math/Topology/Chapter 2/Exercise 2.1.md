![[Exercise211.png]]

*proof:* WLOG we show that $(a,b]$ is not an open subset of $\mathbb{R}$. We choose the special point $b$ and try to find real numbers $c,d$ that satisfy property $(*)$ from the [[The Euclidean Topology on Real numbers|euclidean topology on real numbers]]. Suppose such $a,b$ exists where $b\in(c,d)\subseteq(a,b]$ then $c<b<d\implies c<b<\frac{b+d}{2}<d$. Clearly $\frac{b+d}{2}\in (c,d)$ but $\frac{b+d}{2}\notin (a,b]$. Therefore $(c,d)\nsubseteq(a,b]$. The arguements for $[a,b)$ are similar.

We now try to show $(a,b]$ is not closed by showing $\mathbb{R}\backslash(a,b]=(-\infty,a]\cup(b,\infty)$ is not open. We choose to see if we can find real numbers $c,d$ such that $a\in(c,d)\subseteq(-\infty,a]\cup(b,\infty)$. Same arguments as above can be made to show this is not possible due to contradictions.

![[Exercise212.png]]
The $\mathbb{R}\backslash[a,\infty)=(-\infty,a)$ which is proven to be open in [[Open Sets and Closed Sets in The Euclidean Topology|here]]. Same argument for $\mathbb{R}\backslash(-\infty,a]=(a,\infty)$. So both the sets are closed.

![[Exercise213.png]]
Example $$\bigcup_{n=1}^{\infty}[-(1+\frac{1}{n})^n,(1+\frac{1}{n})^n]=(-e,e).$$

![[Exercise214.png]]

1. We cannot create open intervals (a,b) that are subsets of $\mathbb{Z}$. Because a subset of $\mathbb{Z}$ might look like $\{2,4,6,...\}$.
2. Since $\mathbb{R}\backslash\mathbb{P}=\bigcup_{n=1}^{\infty}(p_i,p_{i+1})$ where $p_i$ is the $i$ th prime number. Clearly it is a closed set in $\mathbb{R}$
3. We cannot create open intervels (a,b) that are subsets of $\mathbb{I}$ because between any two irrational numbers there is a rational number. Meaning there are gaps if we only consider irrational numbers. Therefore it is not open. Looking at $\mathbb{R}\backslash\mathbb{I}$ suffers from the same issue. We cannot create open intervels (a,b) that are subsets of $\mathbb{R}\backslash\mathbb{I}$ because between rational numbers there is an irrational number. Therefore there are gaps in $\mathbb{R}\backslash\mathbb{I}$ which does not make it continuos.

![[Exercise215.png]]
*proof:* Let $F$ have elements $f_1,...,f_n$. Then $\mathbb{R}\backslash F=\bigcup_{i=1}^{n}(f_1,f_n)$ which is an open set in the topology. Take $f_i$ and take and real numbers such that $a<f_i<b$. Therefore $f_i\in(a,b)$ then clearly $(a,b)$ is an infinite set and the $F$ is a finite set. Therefore any $(a,b)\nsubseteq F$.

![[Exercise216.png]]
*proof:* Let $F$ have elements $f_1,f_2,f_3,...$ with $f_1<f_2<f_3<...$ Then take $f_i\in F$. We can create interval $(f_{i-1},f_{i+1})$. Clearly $f_i\in F$. We also know $f_{i-1}<f_{i}<(f_i+f_{i+1})/2<f_{i+1}\implies (f_{i}+f_{i+1})/2\in(f_{i-1},f_{i+i})$ but $(f_{i}+f_{i+1})/2\notin F$. Therefore $(f_{i-1},f_{i+i})\nsubseteq F$. Furthermore, we know that if we choose realnumbers such that $f_{i-1}<a$ and $b<f_{i+1}$ then $f_i\in(a,b)$ but again we can create $\frac{f_i+b}{2}\in(a,b)$ but $\frac{f_i+b}{2}\notin F$. Therefore $(a,b)\nsubseteq F$. Therefore $F$ is not an open set.

We know show that $F$ may or may not be closed. We have examples of $\mathbb{N}$ being closed and $\mathbb{Q}$ not being closed. We have not found any conditions that ensure the set is closed or not closed.

![[Exercise217.png]]

1. The set $\mathbb{R}\backslash S=(-\infty,0)\cup(0,1)\cup\bigcup_{n=1}^{\infty}(1/n,1/(n+1))$ the union of open sets is still an open set.
2. $\mathbb{R}\backslash T = (-\infty,0)\cup\bigcup_{n=1}^{\infty}(1/n,1/(n+1))$. These sets are still open.
3. $\mathbb{R}\backslash \{\sqrt{2},2\sqrt{2},3\sqrt\{2\},...\}=(-\infty,\sqrt{2})\cup\bigcup_{n=1}^{\infty}(n\sqrt{2},(n+1)\sqrt{2})$ is open. Meaning that the set is closed.

![[Exercise218.png]]
1. *proof:* Let $(\mathbb{R},\tau)$ be [[The Euclidean Topology on Real numbers|euclidean topology on real numbers]]. Let $a,b\in\mathbb{R}$ with $a<b$. Then we show that open interval $(a,b)$ is a $F_{\sigma}-$set because $$\bigcup_{i=1}^{\infty}[a+\frac{1}{n},b-\frac{1}{n}]=(a,b).$$ The closed sets $[a,b]$ are also $F_\sigma-$sets because $$\bigcup_{i=1}^{\infty}[a,b]=[a,b].$$
2. *proof:*  Let $(\mathbb{R},\tau)$ be [[The Euclidean Topology on Real numbers|euclidean topology on real numbers]]. Let $a,b\in\mathbb{R}$ with $a<b$. Then we show that open interval $(a,b)$ is a $G_{\delta}-$set because $$\bigcap_{n=1}^{\infty}(a-\frac{1}{n},b+\frac{1}{n})=(a,b).$$ **At the moment cannot figure out how to get a closed interval from a countable number of intersections from open sets.**
