## Zoom in scene
What is a manifold? Well I can show you (circle appears). This is a manifold. Now you might ask "Why is a circle a manifold?". This because of two reasons: the first reason is because the circle is flat. What I mean by this if I have a point on the circle and I start zooming onto the point we see that the region around the point becomes flat. If I go to another point on the manifold and start zooming in we see the that the region become flat.  Exactly like how we perceive the Earth being flat.  All manifolds have this flatness property.

## Charts
Let us talk about the second property. All manifolds come with charts. What are these charts? For the case of a circle they are straight lines that we can cover the circle with. We can have multiple lines that can overlap with each other when we stick them on the circle. The important thing is that we have enough of these lines so that the entire circle is covered. If we had a higher dimensional surface for example a sphere we would have planes that we stick onto the sphere.

 Now we have charts but what are they useful for? Let us place all the charts around the circle. Then let us highlight the region these charts cover on the circle. At the moment I have made these charts translucent, let me remove the white circle so that we can focus  on the regions. We can see regions where these charts overlap. 

Now let me place a point on the circle this point would appear on the right chart. If we slowly move the point to the region where the right and top chart meet we see that the point appears on both the lines. In this region we can use any of the two charts to describe the position of the point on the circle.


## Scene 7
This scene introduces the definition of a circle and explicitly defines the charts.

So far I have talked about these charts quantitatively. Lets bring numbers into the picture and explicitly define these four charts. First I will define the circle, it is a set $\mathit{C}^1$ that of tuples. The numbers in the tuple both belong to $\mathbb{R}$ and they satisfy the following relation. 

We can then define the four charts we had in the following manner. They  take a tuple from the set $\mathit{C}^1$ and map it to a real number.  We will call the four charts the right, top, left and bottom charts. We explicitly define them in the following manner: the right chart takes a tuple (x,y) and maps it to y; the top chart takes a tuple (x,y) and maps it x; the map left map takes a point (x,y) and maps it to y; finally the bottom map takes a tuple (x,y) and maps it to x. It is important to note that this is not the only way to define charts.

## Scene 8

Now that we have explicitly defined the charts let us look at what does it mean. Let us start with the circle. I will place a point on the circle and in the center write out which tuple the position of the point corresponds to. At the moment the position of the point corresponds to tuple (1.00,0.00). Let us slowly move the point around the circle until we reach back to the starting point.  Each position on the circle corresponds to one unique tuple.

We can then bring in the charts.  As before I will highlight the regions of the circle that these charts cover . I will place the point on the chart with its current coordinate. Notice that all the other chart values are question marks. This is because the point is not in their region. Now let us move the dot around the circle slowly.  We see that the y-value of the  tuple and the value of the chart are always equal. Once we enter the region where the right and top chart meet we see that the top chart also has a value. It is equal to the x-value of the tuple. Let us continue moving the point around the circle. 

To conclude a manifold must have two properties. It must be locally flat and it must come with enough charts to cover the entire the manifold.

Thank you for watching the video.