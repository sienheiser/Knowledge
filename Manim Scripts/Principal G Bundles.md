Hello, today we will be constructing our first principal G bundle using the cylinder projected to a circle that I defined in my previous videos. As usual we will look at the the definition of a principal G bundle. Now this is a lengthy definition so I will break this video into three parts to explain each point. 

Hello, today we will be constructing our first principal G bundle. As usual we will look at  the definition of a principal G bundle. Now this is a lengthy definition so I will break this video into parts where I will first explain what is a right G-space, then what it means for a G-space to free and finally talk about quotient spaces.

### Not talk about lie group
We start with explaining right $G$-Spaces. Its definition says Let G be a lie group and E a smooth manifold. Then the map with the left triangle symbol is called a right G-action on E if it satisfies the following conditions. Once these conditions are satisfied we call $E$ a right $G$-Space. 

To explain these conditions we will use the cylinder, so $E=\mathcal{C}^1\times \mathbb{R}$. To clearly define a right action we need to use numbers. Any time we need numbers on a manifold we need to use charts. Let us define a chart on this manifold, we start by placing circles at different heights of the cylinder, then we place vertical lines. 

Let us bring in a red dot and track its coordinates in this chart. At the top it has the following coordinates. If we move the point down the coordinates change in the following manner: as the point reaches each circle, the last coordinate changes by 0.5.

The first two coordinates change when the red dot moves along a circle. Let us bring our dot back to its starting point. We can now define our right $G$-action. If we take a real number -1 our right g action just subtracts from the last coordinate. We can look at a few more numbers. This right g action satisfies all the conditions of the definition and that is it!


## Free Space
We will now talk about Free Space. The principal G-bundle definition talked about our right G-space being a free space. To understand this we define the following set $S_p$. Essentially it collects all the actions that do not move a point on the manifold. We call this set a stabilizer.  Now if for all points of the manifold their stabilizer just contains the identity of the group then we have a free space.

Let us look at the cylinder example; we start with the point up here then we do the following right action. The point moves down, therefore -1 does not belong to stabilizer, now let's move back to our starting point and do a right action with another number. The point still moves. Therefore -0.5 is not part of the stablilizer of this point. Finally, let do a right action with 0. The point does not move, meaning 0 is part of our stablizer. In addition, zero is also the identity of the group we choose. Furthermore, what we did for this single point holds true for all points on the cylinder. There, we have a free space. 

## Intermediate Summary
Let us have an intermediate summary. In the principal G-bundle definition we have done the following; we have constructed a right G-space by defining the following right G-action: we take a real number and do addition on the last coordinate. Furthermore we have shown that this right G-space is a free space. What is remaining is the third point, before we can show that there is a bundle morphism we need to construct a quotient space for our example. 


## Bundle Morphism

Before we can talk about bundle morphisms we have to talk about the following: what is this space down here and what is this $\rho$?
## Quotient Space
 
I will give an example of how we construct our quotient space. Let us start with a cylinder and choose a point $p_0$. We can draw a vertical line through the point. If we take any blue point on this line we can always use the right action we defined to move the blue point to the red point. With this in mind we define the following set. It contains all the points on the vertical line. Now if we choose other points on the cylinder we can then draw vertical lines through these other points and define the following sets. If we collect them into a set we get our quotient space. If we remove the cylinder these point may seem random. If we bring back our cylinder and shift these points along the lines then we see that we get a circle. We have found that our quotient space looks like a circle. 

We can then define the projection $\rho$ in the following manner: take any point $q$ and map to $\mathcal{O}_p$ where $q\in\mathcal{O}_p$.


## Bundle Morphism Complete

We now see that if we start with the following bundle that has the right G-action we defined, our quotient space and projection looks like this. These two bundles look the same. Therefore we have a bundle morphism between the two bundles. As a result we have constructed our first principal g-bundle.

