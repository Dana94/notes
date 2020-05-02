# Wrapping Mesh around Circle Curve

Wrapping an object around a cylinder.

I created an object using the **mesh &gt; circle object** and extruded the edges.

The image shows the back of it to show there is no face behind it, only in the front.

![](../../.gitbook/assets/image%20%2813%29.png)

There needs to be a curve for the circle object to follow to wrap it correctly.

Create a curve with **Shift + A &gt; Curve &gt; Circle**

The circle is selected in the image and wrapped around the cylinder.

![](../../.gitbook/assets/image%20%281%29.png)

Selecting the circle object \(not the circle curve around the cylinder\) assign it a **deform &gt; curve modifier**.

Select **BezierCircle** as its curve.

![](../../.gitbook/assets/image%20%2843%29.png)

I'm not sure the best way to explain this next part, but in edit mode the circle object needs to be moved around until it aligns with the circle curve and wraps itself around it. In the image below I extruded the sides more and raised the center so it would be seen on the cylinder as the circle curve causes the front face to curve in a bit.

![](../../.gitbook/assets/image%20%2836%29.png)

Wiht the culinder showing:

![](../../.gitbook/assets/image%20%2825%29.png)

Reference: [https://blender.stackexchange.com/questions/6226/whats-the-simplest-way-to-wrap-extruded-text-around-a-cylinder](https://blender.stackexchange.com/questions/6226/whats-the-simplest-way-to-wrap-extruded-text-around-a-cylinder)

