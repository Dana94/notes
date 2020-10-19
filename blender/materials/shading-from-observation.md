# Shading From Observation

1. Is it transparent?
2. It is metallic? Glossy shader would do most of this.

### Ceramic

Diffuse and Glossy used.

Diffuse will be underlying color used. Sharp reflections from Glossy on top of that.

When using mix shader, isolate one material at a time to make sure it's purpose is being used. Like the Glossy is used to mirror subtle reflections of the object's environment.

How much Glossy = How much saturation in the reflections.

![](../../.gitbook/assets/image%20%2865%29.png)

### Rubber Tire Material

Soft and malleable.

There is a light spread across the material. So only a Diffuse material isn't a good idea.

Don't set Diffuse to pure black.

Gives nice overall gradient of Diffuse with slightly sharper gradation.

![](../../.gitbook/assets/image%20%2864%29.png)

### Leather Jacket Material

Did not change Diffuse value from previous example.

![](../../.gitbook/assets/image%20%2858%29.png)

### Jean Material

Cloth has tiny little hairs everywhere.

Velvet for cloth.

Translucent for some light shining through the material.

![](../../.gitbook/assets/image%20%2860%29.png)

