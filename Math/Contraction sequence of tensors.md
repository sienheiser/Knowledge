---
aliases: [contraction sequence of tensors]
___

#math 
#TensorNetworks 
![[SequenceOfContraction.jpg]]

Depending on the sequence of contraction chosen the complexity of the problem might increase or decrease. 

Example
In the above figure we have a tensor network. There are two sequences of contraction: top and bottom. In the top sequence we circle the two tensors we contract first. Notice that our circle cuts through four indices. If each index has dimension $D$ then the complexity is $\mathcal{O}(D^4)$. In the second step, the circle still cuts through four indices. Overall, the top sequence has a complexity of $\mathcal{O}(D^4)$. 

In the bottom sequence, we contract the bottom two tensors of the triangle, our rectangle (was a circle) cuts through five indices giving the first step a complexty of $\mathcal{O}(D^5)$. In the second step the rectangle cuts through 4 indices giving the contraction a complexity of $\mathcal{O}(D^4)$. Overall, the complexity of the bottom sequence is $\mathcal{O}(D^5)$.