---
aliases: [logical operators]
---
Here we define the different logical operators.

Uniary operators: Operators that only take one [[Propositional logic|proposition]] and return true or false. 

 | $p$ | $\neg p$ | $\text{ID}_p$| $\text{T}$_p|$\bot$ p
 | ------- | ---------- | --- | --- |
 | t | f | t | t | f |
 | f | t | f | t | f |

Binary operators: Operators that only take two propositions and return true or false

| $p$ | $q$ | $p\land q$ | $p\lor q$ | $p\lxor q$ | $p\implies q$ | $p\iff q$ |
| - | - | --- | --- | ------ | ------ | ------- |
| t | t | t | t | f | t | t |
| t | f | f | t | t | f | f |
| f | t | f | t | t | t | t |
| f | f | f | f | f | t | t |

Higher order operators can be constructed from the NAND operator.


 
 