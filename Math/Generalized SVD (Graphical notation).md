#math 
#TensorNetworks 

We can represent a simple [[Singular Value Decomposition SVD|SVD]] in tensor network notation (shown in [[Graphical notation SVD]]). Suppose we have a tensor that has indices $i$, $j$, $k$ and $l$. Then if we want to perform a SVD between the $l$ index and the rest of the index we must define a [[bijective]] map that groups index $i$, $j$ and $k$ into one index $I$. Once done we reduce the problem to a matrix with index $I$ and index $l$, we can use the notation shown in [[Graphical notation SVD]]. The scheme in graphical notation is shown below

![[GeneralizedSVD.jpg]]


After the first equality we use the inverse of $f$ (where $f$ is a bijective map) because $f^{-1}(I) = (i,j,k)$. Then for the second equality we use SVD. Finally, in the last equality we use the map to get back the indices. 