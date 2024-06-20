We want to find the general Lorentz tranformation. Suppose we have some spacetime vector $S^{\alpha}$. After we boost into a general direction $S^{\alpha}$ gets transformed into $S'^{\alpha}$. We want to find the relations between the two spacetime vectors. The  spatial part of vector $S'^{\alpha}$ can be decomposed into two vectors one that is perpendicular to the direction of the boost and the other that is parallel to the direction of the boost.

$$
S'^{i} = S'^{i}_{\perp}+S'^{i}_{\parallel}
$$

We know that 

$$
S'^{0} = \gamma\beta^{\mu}S_{\mu}
$$
where $\beta^{\mu} = [1,v_x,v_y,v_z]^T$. This is analogous to the Lorentz boost along the x direction only.  The perpendicular components of $S'^{i}$ do not change. The parallel components $S'^{i}$ change as 

$$
S'^{i}_{\parallel} = \gamma(S^{i}-\beta^{i}t).
$$
this is again analogous to the case of Lorentz boosting along one direction. Therefore for the spatial components we get
$$
S'^{i} = S'^{i}_{\perp}+S'^{i}_{\parallel} = S^{i}_{\perp} + \gamma (S^{i}-\beta^{i}t).
$$
The perpendicular component can be rewritten as $S^{i}_{\perp} = S^{i}-S^{i}_{\parallel}$ and $S^{i}_{\parallel} = \frac{\beta^{j}S_{j}}{\beta^{j}\beta_{j}}\beta^{i}$. This gives

$$
S'^{i} = S^{i} + \frac{(\gamma-1)\beta^{j}S_{j}}{\beta^{j}\beta_{j}}\beta^{i} - t\gamma\beta^{i}
$$
which gives matrix equation
![[GeneralLorentzTransformation.png]]