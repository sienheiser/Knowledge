#DifferentialGeometry
### Scaling curves
We will show that 
$$
\exists \tau| \alpha\odot \mathcal{v}_{\gamma,p} = \mathcal{v}_{\tau,p}
$$
i.e. there exists a curve $\tau$ on the manifold such that scaling a curve $\gamma$ gives the same velocity of $\tau$ at point $p$.

Suppose we have a curve $\gamma$ that passes through point $p$ on the manifold and $\gamma(\lambda_0) = p$. Define $\tau(\lambda):= \gamma(\alpha\lambda+\lambda_0)= (\gamma\circ\mu_\alpha)(\lambda)$. Where the second equality is just rewriting the definition in terms of compositions. Therefore $\mu_\alpha(\lambda) = \alpha\lambda+\lambda_0$. Meaning $\tau(0) = \gamma(\lambda_0) = p$. Then lets take $\mathcal{v}_{\tau,p}:= (f \circ \tau)'(0) = (f\circ \gamma\circ \mu_\alpha)'(0)$. 

Now we have to be careful, we are taking the derivative w.r.t $\lambda$. ***Not sure if undergraduate notions work*** but we can rewrite the above expression as


$$
\begin{aligned}
(f\circ \gamma\circ \mu_\alpha)'(0) &= \frac{d([f\circ \gamma]\circ \mu_\alpha)}{d\lambda}\\
&= \frac{d(f\circ\gamma)}{d\mu_\alpha}|_{\mu_\alpha = \lambda_0}\cdot \frac{d\mu_{\alpha}}{d\lambda}|_{\lambda = 0}\\
&= (f\circ \gamma)'(\lambda_0)\alpha \\
&:= \alpha \mathcal{v}_{\gamma,p} 
\end{aligned}
$$
The reason for having $\lambda_0$ in the second equality is because $\mu_{\alpha}(0) = \lambda_0$. In the last equality we have shown that we obtain $\mathcal{v}_{\gamma,p}$.

### Adding Curves

For adding curves the strategy is to introduce a chart then add the define a curve that might satify addition of two curves in the chart.  ***Will do later!!***