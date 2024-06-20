
#ClassicalMechanics 
With the setup described in [[Elastics Collisions (CM)| elastic collisons (CM)]]. We may find the relations of momentum after collisions in the L frame. We know that
$$
\vec{v}_1' = \vec{v}_{01} ' + \vec{V}, \quad \vec{v}_2' = \vec{v}_{02}' + \vec{V} \tag{1}
$$
where $v_{01}'$ is the velocity of the particle after collisions in the CM frame, similar definition for $v_{02}'$. We know from [[Two-Body problem reduction|two-body problem reduction]] that $\vec{V} = \frac{\vec{p}_1+\vec{p}_2}{m_1+m_2}$. We may write the above equations in terms of the momentum giving

$$
\vec{p}_1' = \vec{p}_{01} ' + m_1\frac{\vec{p}_1+\vec{p}_2}{m_1+m_2}, \quad \vec{p}_2' = \vec{p}_{02}' + m_2\frac{\vec{p}_1+\vec{p}_2}{m_1+m_2}. \tag{2}
$$

Geometrically the above equation may be represented as 

![[General Elastic Collision.jpg]]

where $\chi$ is the angle between the $\vec{v}_{01}'$ and $\vec{V}$ and $m = m_1m_2/(m_1+m_2)$. To simplify the following case we can set the velocity of the particle with mass $m_2$ to be zero in the L frame. Then it is clear that $OB = mv$ since $v_1 = v$.  We get the following diagrams 

![[Elastic Collision Cases.jpg]]
From the above diagram the relation between $\theta_1$ and $\chi$ is 

$$
\tan(\theta_1) = \frac{mv\sin(\chi)}{\frac{m_1^2}{m_1+m_2}+mv\cos(\chi)} = \frac{m_2\sin(\chi)}{m_1+m_2\cos(\chi)}, \quad \theta_2 = \frac{1}{2}(\pi-\chi) \tag{3}
$$

***If $m_1<m_2$ then $\theta_1+\theta_2 > \frac{\pi}{2}$, if $m_1> m_2$ then $\theta_1+\theta_2 < \frac{\pi}{2}$.  Not sure how this is true***. Furthermore from the above diagram we can see that if $m_1 < m_2$ then the direction of $m_1$ after collision can be in any direction. If $m_1 > m_2$ then there is a max angle above which the mass $m_1$ will not go. The relation between the max angle and the masses is given as

$$
\sin(\theta_{\text{max}}) = \frac{OC}{OA} = \frac{m_2}{m_1} \tag{4}
$$

Using that equations (1) with the fact $v_{01} = m_2v/(m_1+m_2)$ and $V = m_1v/(m_1+m_2)$ we may compute magniuted of $v_1'$ and $v_2'$ purely in terms of masses, $\chi$ and $v$. We get the following relations

$$
\begin{aligned}
v_1' &= \sqrt{m_1^2+m_2^2+2m_1m_2\cos(\chi)} \frac{v}{m_1+m_2}\\
v_2' &= \frac{2m_1v}{m_1+m_2}\sin(\frac{\chi}{2}). 
\end{aligned}
\tag{5}
$$



