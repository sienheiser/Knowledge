## Abstract
In this note we define the $(C^1\times\mathbb{R},\pi,C^1)$ bundle and the Cartesian charts for the manifolds $C^1\times\mathbb{R}$ and $C^1$.

## Introduction

The general definition of bundles can be found [[Physics/Lectures on Geometrical anatomy on Theoretical physics/Lecture 6/Bundles|here]]. We would like to construct a bundle using the smooth manifolds $C^1\times\mathbb{R}$ and $C^1$, where $C^1$ is a circle, $\mathbb{R}$ is the set of real numbers and $C^1\times\mathbb{R}$ is a cylinder. To get a bundle given the two smooth manifolds, a projection map $\pi: C^1\times\mathbb{R}\longrightarrow C^1$ that is smooth and surjective needs to be defined.

Since points in $C^1\times\mathbb{R}$ and $C^1$ are abstract we may use charts to further understand how to define a projection between the two manifolds

## Charts

### Cartesian Chart
Since $C^1\times\mathbb{R}$ and $C^1$ are smooths manifolds, they come equiped with charts by definiton. They both a have cartesian chart. The cartesian chart for $C^1\times\mathbb{R}$ is defined as 
 $x_{\mathit{C}^1\times\mathbb{R}}:\mathit{C}^1\times\mathbb{R}\rightarrow \mathbb{R}^3$, where for a $p\in\mathit{C}^1\times\mathbb{R}$ then $x_{\mathit{C}^1\times\mathbb{R}}(p) = (r\cos a,r\sin a,b)$, where $a,b\in\mathbb{R}$ and $r$ is a positive real number. The cartesian chart for $C^1$ is defined as $x_{\mathit{C}^1}:\mathit{C}^1\rightarrow\mathbb{R}^2$  , where for a $q\in\mathit{C}^1$ $x_{\mathit{C}^1}(q) = (s\cos c,s\sin c)$, where $s$ is a positive real number and $c$ is a real number.
 
#### Defining a projection
One possible way to define a projection $\pi:C^1\times\mathbb{R}\rightarrow C^1$ is to take the point $p\in C^1\times\mathbb{R}$ where $x_{C^1\times \mathbb{R}}(p) = (r\cos a,r\sin a,b)$ and define $\pi(p)\in C^1$ to have coordinates $x_{C^1}(\pi(p)) = (r\cos a,r \sin a)$. With this projection $(C^1\times\mathbb{R},\pi,C^1)$ becomes a bundle. 

There are other possible projections, but share a common triat which is removing the third coordinate from $x_{C^1\times\mathbb{R}}$.


