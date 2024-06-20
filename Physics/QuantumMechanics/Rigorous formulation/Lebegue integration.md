We only define it for [[Measureable non-negative functions|measurable non-negative functions]].
	*Definiton:* Let $(M,\sigma,\mu)$ be a [[Physics/QuantumMechanics/Rigorous formulation/Measure|measure space]] and $(\overline{\mathbb{R}},\overline{\sigma})$ be a [[Sigma algebra|measurable space]] where $\overline{\mathbb{R}},\overline{\sigma}$ is defined in [[Measureable non-negative functions|measurable non-negative functions]]. Then the integral $\int f d\mu$ of a measurable non-negative function $f:M\rightarrow \overline{\mathbb{R}}$ is the number ($\in\overline{\mathbb{R}}$)
$$
\int fd\mu := \sup\{\sum_{z\in s(M)}z\cdot \mu(\text{preim}_s({z}))|\text{over all possible simple function  } s\text{ with  }0\leq s\leq f\}	
$$
where we have defined [[Simple function|simple function]]. It is important to have a measure $\mu$ on the domain. 


*Notation:* It is often very convinient to write 
$$
\int_A fd\mu := \int f\cdot \chi_A d\mu
$$
where $\chi_A$ is the [[Characteristic function|characteristic function]] and $\cdot$ is the multiplication between function in function space. Furthermore we may define more notation as
$$
\int fd\mu := \int f(x)\mu(dx).
$$


