#Calculus 

The Dirac delta function $\delta (x)$ is a distribution that is defined to have the following property
$$
\begin{aligned}
\int f(x)\delta(x-a)dx & = f(a).
\end{aligned}
$$

The Dirac Delta function has the following properties

$$
\begin{aligned}
&\text{i)}\quad \int \delta(x)dx  1\\
&\text{ii)} \int \delta(-t)dt = \int \delta(t) dt\\
&\text{iii)} \int t\delta(t)dt = 0\\
&\text{iv)} \int \delta(at)dt = \frac{1}{|a|}\int\delta(x)dx = \frac{1}{|a|}\\
&\text{v)}\quad\delta(h(t)) = \sum_i \frac{\delta(t-t_i)}{|h'(t_i)|}
\end{aligned}
$$
where in v) $h(t)$ is a function with zeros at points $t_1,t_2,....$