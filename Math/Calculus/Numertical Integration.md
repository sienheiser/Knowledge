### 1D integration
Suppose we have a 1D function $f(x)$ and we want to compute its definite integral. This is given by:

$$
\int_a^b f(x)dx = \lim_{N\rightarrow \infty} \sum_{n=1}^{N}\Delta x f(n\Delta x + a ) \quad \text{where} \quad \Delta x = \frac{b-a}{N}.
$$

### 2D integration

Inegrating a 2D function is similar to the 1D function, we get the following equation

$$
\int_{a_x}^{b_x}\int_{a_y}^{b_y} f(x,y)dydx = \lim_{N_x\rightarrow \infty} \lim_{N_y\rightarrow\infty} \Delta x \Delta y\sum_{i = 1}^{N_x} \sum_{j = 1}^{N_y} f(i\Delta x + a_x, j\Delta y + a_y),
$$
where 
$$
\Delta x = \frac{b_x-a_x}{N_x}, \quad \Delta y = \frac{b_y-a_y}{N_y}.
$$

### Computing length of 1D curve 
Suppose we have parametrization of curve $\mathcal{C}$ as $\vec{r}(t)$. Then to compute the lenght of the curve we need $\vec{v} = \frac{d\vec{r}(t)}{dt}$. The following integral computes the lenght of a curve

$$
\int_{t_0}^{t_1} \sqrt{\vec{v}\cdot \vec{v}} dt = \lim_{N\rightarrow \infty} \sum_{n= 1}^N\Delta t f(n\Delta t + t_0) 
$$
where
$$
f(t) = \sqrt{\vec{v}\cdot\vec{v}} \quad \text{and} \quad \Delta t = \frac{t_1-t_0}{N}.
$$