# Changing Texture Coordinates

Direction to give to the texture using Texture Coordinate Node.

* **Generated**: Projecting from top. Top will look normal, but sides will be completely stretched.

Setting the image texture to "Box" will help it project from all 4 sides. This would look good on a cube mesh.

Increase "Blend" to blur the edges.

"Sphere" works well on sphere meshes.

"Tube" for cylinders.

![](../../../.gitbook/assets/image%20%2866%29.png)

* **Object:** Takes the objects location and scales into account as the mesh gets bigger without distorting the texture.
* **Camera**: Points everything towards the camera. \(Set Image Texture to "flat"\).
* **Window**: Stretched over the object.
* **Reflection**: A bit strange, gives a kaleidoscope look.

### Mapping

Tip: Click on value slot and hold down to select others below so their values will all be set to the same new value at once.

![](../../../.gitbook/assets/image%20%2859%29.png)

Good for easily repeatable patterns \(dirt, grass\).

![](../../../.gitbook/assets/image%20%2872%29.png)

