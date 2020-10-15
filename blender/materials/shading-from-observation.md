# Shading From Observation

1. Is it transparent?
2. It is metallic? Glossy shader would do most of this.

### Ceramic

Diffuse and Glossy used.

Diffuse will be underlying color used. Sharp reflections from Glossy on top of that.

When using mix shader, isolate one material at a time to make sure it's purpose is being used. Like the Glossy is used to mirror subtle reflections of the object's environment.

How much Glossy = How much saturation in the reflections.

![](../../.gitbook/assets/image%20%2861%29.png)

