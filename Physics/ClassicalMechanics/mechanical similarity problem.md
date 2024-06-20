#ClassicalMechanics 

Suppose we have look at the case where we throw a ball with initial velocity $v_x$ and $v_y$ in a uniform gravitational field starting at the origin. Then the Lagrangian is given as 

$$
\mathcal{L} = \frac{m}{2}(\dot{x}^2+\dot{y}^2)-mgy
$$
which gives equations of motion

$$
x = v_xt, \quad y = -\frac{gt}{2}+v_yt.
$$

Suppose we multiply the same Lagrangian with constant $\alpha$ since the potential is just a linear homogenous function. Then

$$
\alpha\mathcal{L} = \frac{m}{2}(\alpha\dot{x}^2+\alpha\dot{y}^2)-\alpha mgy = \frac{m}{2}(\dot{x}^{'2}+\dot{y}^{'2})-mgy^{'}
$$
which gives equations of motion
$$
x^{'} = v_x^{'}t^{'}, \quad y^{'} = -\frac{gt^{'}}{2}+v_y^{'}t^{'}.
$$

The lenght of the path can be calculated by 

$$
l = \int_0^{2v_y/g}\sqrt{v_x^2+(v_y-gt)^2}dt.
$$
After rewriting and using wolframalpha we get

$$
l = -\frac{v_x}{2g}\left(v_y\sqrt{\frac{v_y^2}{v_x^2}+1}+v_x\sinh^{-1}(\frac{v_y}{v_x})\right) = -\frac{v_xv_y}{2g}\left(\sqrt{\frac{v_y^2}{v_x^2}+1}+\frac{v_x}{v_y}\sinh^{-1}(\frac{v_y}{v_x})\right).
$$
Similarly for 

$$
l^{'} = -\frac{v_x^{'}}{2g}\left(v_y^{'}\sqrt{\frac{v_y^{'2}}{v_x^{'2}}+1}+v_x^{'}\sinh^{-1}(\frac{v_y^{'}}{v_x^{'}})\right) = -\frac{v_x^{'}v_y^{'}}{2g}\left(\sqrt{\frac{v_y^{'2}}{v_x^{'2}}+1}+\frac{v_x^{'}}{v_y^{'}}\sinh^{-1}(\frac{v_y^{'}}{v_x^{'}})\right).
$$
We see that 
$$
\frac{l}{l^{'}} = \frac{1}{\alpha},
$$
note that this is true for $k = 1$ where $k$ is degree of the homogenous function. We see that all the relations between the ratio of the two paths and different conserved quantities are satisfied in [[Mechanical Similarity|mechanical similarity]].
