
![[Covariant_hom_functor.png]]
The above figure shows objects $X,Y$ and $A$ all of whom belong to a category $C$. We see arrows emanating from $A$ to $X$ and $Y$. We group these arrows into set and call it $\text{Hom}(A,X)$ and $\text{Hom}(A,Y)$. There is also an arrow $f$ that goes from $X$ to $Y$.

We can select any $g\in\text{Hom}(A,X)$ and do the following $f\circ g$ which belongs to $\text{Hom}(A,Y)$. We can view $\text{Hom}(A,-)$ as a functor. We call $\text{Hom}(A,-)$ a hom functor. 

On the right we see objects $\text{Hom}(A,X)$, $\text{Hom}(A,Y)$ and arrow $\text{Hom}(A,f)$ all of whom belong to the category $\text{Set}$. $\text{Hom}(A,X)$ goes by $\text{Hom}(A,Y)$ by simply prepending all the functions in it by $f$; this is what $\text{Hom}(A,f)$ represents. As you can see $\text{Hom}(A,-)$ is a covariant functor.

![[Contravariant_hom_functor.png]]
On the left, the objects in the above figure are the same as in the first figure. The only difference is that the arrows now points $X,Y$ towards $A$. We then get sets $\text{Hom}(X,A)$ and $\text{Hom}(Y,A)$. We now pick a function $v\in\text{Hom}(Y,A)$. If we do the following composition $v\circ f$ we get a function that belongs to $\text{Hom}(X,A)$.

If we view this situation under the lenses of category $\text{Set}$ we get the view on the right side. Notice how arrow represented by $f$ has been reversed after we apply $\text{Hom}(-,A)$ to all the objects and $f$ on the right side. This shows that $\text{Hom}(-,A)$ is a contravariant functor.