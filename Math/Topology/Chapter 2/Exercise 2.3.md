![[Exercise231.png]]
Have the anser written but too lazy to write it again.


![[Exercise232.png]]
**(i)** Since $\mathcal{B}_1\subseteq \tau$ we know that for all $B\in\mathcal{B}_1$, $B\in \tau$. Furthermore since $\mathcal{B}$ is a basis for $\tau$ we know all members of $\tau$ can be made as a union of members $\mathcal{B}$. This means all members of $\mathcal{B}_1$ can be represented as union of members of $\mathcal{B}$. Therefore take $B'_i\in\mathcal{B}_1$ then 
$$
B'_i=\bigcup_{j\in J}B_{ij}\quad \text{where}\quad B_{ij}\in\mathcal{B.}
$$
Since $\mathcal{B}\subseteq\mathcal{B}_1$ all $B\in\mathcal{B}$ also belongs to $\mathcal{B}_1$. This means $\mathcal{B}_1$ has all the necessary members to be a basis for $\tau$.

**(ii)** We know that $\mathcal{B}=\{(a,b)|a,b\in\mathcal{R},a<b\}$ is a basis for [[The Euclidean Topology on Real numbers|euclidean topology on real numbers]]. We can create

$$
\mathcal{B}'=\mathcal{B}\bigcup [(a,b)\cup (c,d)]\quad a,b,c,d\in\mathbb{R}\quad a<b<c<d.
$$
Clearly there are uncountable many elements therefore there are uncountably many basis.



![[Exercise233.png]]
To show that $(a,b)$ is an open set we have to show that it is a union of members of the basis. Take any $x\in(a,b)$. For $x< \frac{a+b}{2}$ create interval $(a-\frac{x-a}{10},\frac{a+b}{2}]$. Clearly, $(a-\frac{x-a}{10},\frac{a+b}{2}]\in\mathcal{B}$. For $x\geq \frac{a+b}{2}$ create $(a,b+\frac{b-x}{10}]$. Clearly, $\frac{a+b}{2}\in\mathcal{B}$. So we have shown for all $x\in (a,b)$ we can find $B\in\mathcal{B}$ such that 
$$
x\in B\subseteq (a,b).
$$
Therefore by proposition [[Basis and open sets|basis and open sets]] $(a,b)$ is an open set in $(\mathbb{R},\tau)$.

![[Exercise234.png]]
We have $X=C[0,1]$ which is the set of all continous real-valued function on $[0,1]$. We define a collection $\mathcal{M}=\{M(f,\epsilon)|f\in C[0,1]\land \epsilon\text{ is a positive real number}\}$. We define $M(f,\epsilon) = \{g|g\in C[0,1]\land \int_{0}^{1}|f-g|<\epsilon\}$.  To show that $\mathcal{M}$ is a basis for a topology we show that 
1. $C[0,1]=\bigcup_{N\in\mathcal{M}}N$. Take any $f\in C[0,1]$. Then we know that $f\in M(f,\epsilon)$ because $\int_0^1|f-f|=0<\epsilon$ for any real positive number. But $M(f,\epsilon)\in\mathcal{M}$. Therefore $f\in\bigcup_{N\in\mathcal{M}}N$. So $C[0,1]\subseteq \bigcup_{N\in\mathcal{M}}N$. Now take $g\in M(f,\epsilon)$. By definiton of $M(f,\epsilon)$ $g\in C[0,1]$. Therefore  $C[0,1]\supseteq \bigcup_{N\in\mathcal{M}}N$. 
Next we need to show that the intersection between any two members of $\mathcal{M}$ is still a union of memebrs of $\mathcal{M}$. #ToBeProven 


![[Exercise235.png]]
Subbasis for a topology. #ToBeProven Also exercises 2.6 to 2.12. 