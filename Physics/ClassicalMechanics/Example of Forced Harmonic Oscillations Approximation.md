#ClassicalMechanics 

### Specific example
In [[Forced Harmonic Oscillations Approximation| forced harmonic oscillations]] we found the equations of motion to be 

$$
\ddot{x} = -\omega^2 x - \frac{F(t)}{m}. \tag{1}
$$

Suppose $F(t) = f\cos(\gamma t + \beta)$. Then to solve equation (1) we have to find the homogenous and particular solutions. The homogenous solution is $x_h(t) = a\cos(\omega t + \alpha)$. The particular solution is $x_p = b\cos(\gamma t-\beta)$ where $b = \frac{f}{m(\omega^2-\gamma^2)}$. So the general solution is 
$$
x = a\cos(\omega t+\alpha)+\frac{f}{m(\omega^2-\gamma^2)}\cos(\gamma t+\beta). \tag{2}
$$
So for small oscillations a system under a weak periodic external force executes a motion that is a combination of oscillations from the system and from the external force.

### Resonance Frequency 
Notice that equation (2) is not valid when $\gamma \rightarrow \omega$. To get a better equation we may add another homogenous solution to $x$ giving
$$
x = a\cos(\omega t+\alpha)+\frac{f}{m(\omega^2-\gamma^2)}[\cos(\gamma t+\beta)-\cos(\omega t+\beta)]. \tag{3}
$$
where $a$ is different from equation (2). Now as $\gamma \rightarrow \omega$ the second term has form 0/0 which means we may use [[L'Hopital's rule]] which gives

$$
x = a\cos(\omega t+\alpha)+\frac{f}{2m\omega}t\sin(\omega t+\alpha) \tag{4}
$$
so the amplitude of $x$ grows linearly in time. This obviously breaks down as the $x$ becomes big.

### Behaviour near resonance frequency
Suppose $\gamma \rightarrow \omega+\epsilon$ where $\epsilon$ is small and positive. Then rewriting equation (2) in complex form and subtituting gamme gives

$$
x = Ae^{i\omega t}+Be^{i(\omega+\epsilon)t} = e^{i\omega t}[A+Be^{i\epsilon t}]. \tag{5}
$$

where $A = a\exp(i\alpha)$ and $B = b\exp(i\beta)$. In a period $T = 2\pi/\omega$ $\exp(i\epsilon t)$ varies very little, ***the motion near resonance may be regarded as small oscillations of variable amplitude***. If we set $C = A+B\exp(i\epsilon t)$ then amplitude is 
$$
C^2 = a^2+b^2+2ab\text{Re}[e^{i(\beta-\alpha)+\epsilon}]
$$

which means that the amplitude varies between $|a-b|\leq C\leq a+b$. This phenomena is known as ***beats***.