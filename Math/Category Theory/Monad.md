Let $C$ be a category. Then the triple $(T,\eta,\mu)$ where $T:C\rightarrow C$ is an endofunctor, $\eta: Id \rightarrow T$ is a natural transformation and $\mu: T\circ T\rightarrow T$ is a natural transformation. The $id$ is a identity functor. So $\eta$ take $id$ to $T$. The tripe above is called a monad if the following conditions are satisfied

1) $\mu\circ T\mu = \mu \circ \mu T$
2) $\mu \circ T\eta = \mu\circ \eta T = 1_T$
where $1_T$ is the identity natural transformation from $T\rightarrow T$
	

<img src="https://i.upmath.me/svg/%24%5Cbegin%7Btikzcd%7D%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%26%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%26%20TTX%20%5C%5C%0AX%20%5Carrow%5Br%2C%20%22%5Ceta_X%22%5D%20%26%20TX%20%5Carrow%5Bru%2C%20%22%5Ceta_%7BTX%7D%22%5D%20%5Carrow%5Brd%2C%20%22T(%5Ceta_%7BX%7D)%22%5D%20%26%20%20%20%20%20%5C%5C%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%26%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%26%20TTX%0A%5Cend%7Btikzcd%7D" alt="$\begin{tikzcd}
                      &amp;                                                      &amp; TTX \\
X \arrow[r, &quot;\eta_X&quot;] &amp; TX \arrow[ru, &quot;\eta_{TX}&quot;] \arrow[rd, &quot;T(\eta_{X})&quot;] &amp;     \\
                      &amp;                                                      &amp; TTX
\end{tikzcd}" />



The above figure is a communitive diagram for $\eta$. When we take and object $X$ from category $C$ then apply $\eta_X$ in the following manner.

<img src="https://i.upmath.me/svg/%24%5Cbegin%7Btikzcd%7D%0AT(T(T(X)))%20%5Carrow%5Br%2C%20%22T(%5Cmu_x)%22%5D%20%5Carrow%5Bd%2C%20%22%5Cmu_%7BT(X)%7D%22%5D%20%26%20T(T(X))%20%5Carrow%5Bd%2C%20%22%5Cmu_X%22%5D%20%26%20%20%26%20T(X)%20%5Carrow%5Br%2C%20%22%5Ceta_X%22%5D%20%5Carrow%5Bd%2C%20%22%5Ceta_%7BT(X)%7D%22%5D%20%26%20T(T(X))%20%5Carrow%5Bd%2C%20%22%5Cmu_X%22%5D%20%5C%5C%0AT(T(X))%20%5Carrow%5Br%2C%20%22%5Cmu_X%22%5D%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%26%20T(X)%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%26%20%20%26%20T(T(X))%20%5Carrow%5Br%2C%20%22%5Cmu_%7BX%7D%22%5D%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%26%20T(X)%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%0A%5Cend%7Btikzcd%7D" alt="$\begin{tikzcd}
T(T(T(X))) \arrow[r, &quot;T(\mu_x)&quot;] \arrow[d, &quot;\mu_{T(X)}&quot;] &amp; T(T(X)) \arrow[d, &quot;\mu_X&quot;] &amp;  &amp; T(X) \arrow[r, &quot;\eta_X&quot;] \arrow[d, &quot;\eta_{T(X)}&quot;] &amp; T(T(X)) \arrow[d, &quot;\mu_X&quot;] \\
T(T(X)) \arrow[r, &quot;\mu_X&quot;]                               &amp; T(X)                       &amp;  &amp; T(T(X)) \arrow[r, &quot;\mu_{X}&quot;]                      &amp; T(X)                      
\end{tikzcd}" />

The above diagram shows the relations 1) and 2).

## Applying monad to Haskell
### Writer problem
In category $C$ suppose we have objects $a, b, c, Ta, Tb$ and $Tc$; morphisms $f:a \rightarrow Tb$ and $g:b \rightarrow Tc$. Suppose we want to define composition $g\circ f$ to do this we can use monads. Let $C$ have a monad $(T,\eta,\mu)$. Then we can do the following operations

 <center>
<img src="https://i.upmath.me/svg/%24%5Cbegin%7Btikzcd%7D%0Aa%20%5Carrow%5Brr%2C%20%22%5Ceta_a%22%5D%20%5Carrow%5Brrd%2C%20%22f%22%5D%20%26%20%20%26%20Ta%20%5Carrow%5Brrd%5D%20%5Carrow%5Brr%2C%20%22%5Ceta_%7BTa%7D%22%5D%20%20%20%20%20%20%20%20%20%26%20%20%26%20TTa%20%5Carrow%5Brr%2C%20%22%5Cmu_a%22%5D%20%26%20%20%26%20Ta%20%5C%5C%0Ab%20%5Carrow%5Brrd%2C%20%22g%22%5D%20%5Carrow%5Brr%2C%20%22%5Ceta_b%22%5D%20%26%20%20%26%20Tb%20%5Carrow%5Brrd%2C%20%22T(g)%22%5D%20%5Carrow%5Brr%2C%20%22%5Ceta_%7BTa%7D%22%5D%20%26%20%20%26%20TTb%20%5Carrow%5Brr%2C%20%22%5Cmu_b%22%5D%20%26%20%20%26%20Tb%20%5C%5C%0Ac%20%5Carrow%5Brr%2C%20%22%5Ceta_c%22%5D%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%26%20%20%26%20Tc%20%5Carrow%5Brr%2C%20%22%5Ceta_%7BTc%7D%22%5D%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%26%20%20%26%20TTc%20%5Carrow%5Brr%2C%20%22%5Cmu_c%22%5D%20%26%20%20%26%20Tc%0A%5Cend%7Btikzcd%7D" alt="$\begin{tikzcd}
a \arrow[rr, &quot;\eta_a&quot;] \arrow[rrd, &quot;f&quot;] &amp;  &amp; Ta \arrow[rrd] \arrow[rr, &quot;\eta_{Ta}&quot;]         &amp;  &amp; TTa \arrow[rr, &quot;\mu_a&quot;] &amp;  &amp; Ta \\
b \arrow[rrd, &quot;g&quot;] \arrow[rr, &quot;\eta_b&quot;] &amp;  &amp; Tb \arrow[rrd, &quot;T(g)&quot;] \arrow[rr, &quot;\eta_{Ta}&quot;] &amp;  &amp; TTb \arrow[rr, &quot;\mu_b&quot;] &amp;  &amp; Tb \\
c \arrow[rr, &quot;\eta_c&quot;]                  &amp;  &amp; Tc \arrow[rr, &quot;\eta_{Tc}&quot;]                     &amp;  &amp; TTc \arrow[rr, &quot;\mu_c&quot;] &amp;  &amp; Tc
\end{tikzcd}" />
</center>
Suppose we want to compose functions $g\circ f$. We can do the following 
$$
g\circ_T f = \mu_c\circ T(g) \circ f
$$
In haskell we can do the following

```
-- Define the Writer type alias
type Writer a = (a, String)

-- Functor instance
instance Functor Writer where
  -- fmap :: (a -> b) -> Writer a -> Writer b
  fmap f (a, s) = (f a, s)

-- Monad instance
instance Monad Writer where
  -- return :: a -> Writer a
  return a = (a, "")
  
  -- (>>=) :: Writer a -> (a -> Writer b) -> Writer b
  ma >>= f = join (fmap f ma)
    where
      -- join :: Writer (Writer a) -> Writer a
      join (Writer (a, s2), s1) = (a, s1 ++ s2)
```

In the monad implementation above we have defined $\eta$ and $\mu$. The return function does the role of $\eta$ and the join function does the role of $\mu$. So depending on the case $\eta$ and $\mu$ changes. 

So if you want to compose two functions f and g we can define the following operator
```
(>=>) :: (a->mb) -> (b -> mc) -> (a -> mc)
f >=> g = let \a->
	mb = f a
	in mb >>= g
```
So now we have defined a new composition between two functions.

