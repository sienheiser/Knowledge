In principle we can choose any scheme but take 
1. $\Im\langle e_{n\delta},e_{n\delta}(\lambda)\rangle = 0\forall \lambda \in (a,b)$.
2. $||e_{n\delta}(\lambda)||^2 = 1$

Inserting the above condition into [[Formal power series ansatz|ansatz]] gives the following equation
1. $\Im\langle e_{n\delta},\epsilon^{(k)}_{n\delta}\rangle = 0$
2. $0 = 2\lambda\Re\langle e_{n\delta},\epsilon^{(i)}_{n\delta}\rangle+\lambda^2(2\Re\langle e_{n\lambda},\epsilon_{n\delta}^{(2)} \rangle)+||\epsilon_{n\delta}^{(1)}||^2+\mathcal{O}(\lambda^3)$

The conclusions that can be drawn from the above equations are

1. $\langle e_{n\delta},\epsilon^{(1)}_{n\delta}\rangle = 0$
2. $\langle e_{n\delta},\epsilon^{(2)}_{n\delta}\rangle = -\frac{1}{2}||\epsilon^{(1)}_{n\delta}||^2$

Which finally give us relations
1. $\epsilon^{(1)}_{n\delta}\perp e_{n\delta}$
2. $\epsilon^{(2)}_{n\delta} = -\frac{1}{2}||e^{(1)}||^2e_{n\delta}+$ contribution from $\text{span}(e_{n\delta})$.