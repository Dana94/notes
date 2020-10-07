# The Subsurface Scattering Shader

Candle wax like texture.

Light travels through the object, but bounce around inside of it.

* scale: how far the light can travel \(set to 0 mirrors diffuse mode\) the higher it gets to 1, the softer the edges are.
* radius: 3 values \(red, green, blue\) Creates a tint, otherwise set all to 1 to make them the same.
* Technique: Default is **Christensen-Burley**, which is good but **Random Walk** is more accurate because it preserves hard edges much better.

**Shift + S** while clicking on a node to swap it out with another.

Thick material will usually want to use subsurface scattering.

Candle material:

![](../../.gitbook/assets/image%20%2852%29.png)



