Suppose we have some distribution of matter that creates a field. If $\vec{r}'$ parametrizes the distrubution of the source then the vector $\vec{r}-\vec{r}'$ points from the source to a position in space. If the magnitude $r>>r'$ then the following approximation can be made:
$$
|\vec{r}-\vec{r}'| = \sqrt{r^2+r'^2-2rr'\cos\alpha} = r\left( 1 +\frac{r'^2}{r^2}-\frac{2r'}{r} \cos\alpha\right)
$$
$$
\approx r \left(1-\frac{2r'}{r} \cos\alpha \right) = r-\hat{\vec{r}}\cdot \vec{r}'
$$

where 

$$
\hat{\vec{r}} = \frac{\vec{r}}{r}.
$$

Usually when dealing with waves we have functions of form

$$
f(\vec{x},\vec{x}')=\frac{\exp(\pm ip|\vec{r}-\vec{r}'|/\hbar)}{|\vec{r}-\vec{r}'|}\approx \frac{\exp(\pm ik/\hbar)\exp(\mp i \vec{k}'\cdot\vec{x}'/\hbar)}{r} 
$$
where we replaces $|\vec{r}-\vec{r}'|\approx  r$ for big $r>>r'$, $k = pr$ and $\vec{k}' = p\hat{\vec{r}}$