---
aliases: [tensor network diagrams]
---


#math 
#TensorNetworks


We know what is a [[Tensor|tensor]]. They can contract with each other to form other tensors. Here we introduce new graphical notation for tensors. 

### Tensor diagram rules 

![[TensorNetworkDiagram.jpg]]
1. Tensors are notated by solid shapes, and tensor indicies are notated by lines emnating from these shapes.
2. Connecting two index lines implies a contraction, or summation over the connected indices.

Example is shown in the figure above. In the first case we have tensor $C_{ij}$ made from a contraction between tensors $A_{ik}B_{kj}$. The second one is a ring since a trace sums over all the indicies. This notation also shows the cyclic nature of the trace.


