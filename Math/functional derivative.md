---
aliases: [functional derivative]
---
#math 
The concept of functional derivatives come the calculus of varation (see variational principle). Suppose we have some functional $F[f]$. We can define the the functional derivative by varying the function $f$ infinitesimally i.e. $f\rightarrow f+\epsilon\eta$ where $\epsilon$ is an infinitesimal parameter and $\eta$ is a nice function that depends on the same variables as $f$. Then we can expand the function $F[f+\epsilon\eta]$ in terms of $\epsilon$. We Taylor expand (see [[Taylor expansion used in physics|Taylor expansion in physics]]) with $\epsilon =0$ giving

$$
F[f(x)+\epsilon\eta(x)] = F[f(x)] + \frac{dF[f(x)+\epsilon\eta(x)]}{d\epsilon}|_{\epsilon = 0} \epsilon + \text{higher order terms}.
$$

The 1st order functional derivative is defined to be 
$$
\frac{dF[f(x)+\epsilon\eta(x)]}{d\epsilon}|_{\epsilon = 0}.
$$
This functional derivative can be written as 
$$
\frac{dF[f(x)+\epsilon\eta(x)]}{d\epsilon}|_{\epsilon = 0} = \int \frac{\delta F}{\delta f(x)}\eta(x)dx
$$
### Example for functional derivatives
In quantum mechanics we have potential term from the [[Schrodinger equation]]

$$
<\psi|\hat{V}|\psi> = \int \psi^*(x)V(x)\psi(x)dx
$$
where $|\psi>$ is the state ket and $\hat{V}$ is the potential. The RHS is written in coordinate representation. In fact the RHS is a functional
$$
F[\psi,\psi^*] = \int \psi^*(x)V(x)\psi(x)dx.
$$

The first order derivative of the functional w.r.t $\psi^*$. Then

$$
\frac{F[\psi(x),\psi(x)^*+\epsilon\eta(x)]}{d\epsilon}|_{\epsilon = 0} =  \frac{d}{d\epsilon}\int (\psi^*(x)+\epsilon\eta(x))V(x)\psi(x)dx = \int \eta(x)V(x)\psi(x)dx.
$$

Notice that $\int \eta(x)V(x)\psi(x)dx$ has same form as $\int \frac{\delta F}{\delta f(x)}\eta(x)dx$ if $\frac{\delta F}{\delta f(x)} =V(x)\psi(x)$ with $f(x) = \psi^*(x)$.

### usefulness of functional derivates
See [[Gross-Piteavski equation#Derivation of GPe equation]] for a proper application.