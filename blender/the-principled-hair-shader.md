# The Principled Hair Shader

2 shaders you can use:

**Hair BSDF**

Has 2 options: Reflection \(light is bouncing off of hair\) or Transmission \(light is scattering though the hairs\)

Typically use 2 of these shaders and mix the 2 options for the hair material.

**RoughnessU**: The roughness along th hair and down the strand.

**RoughnessV**: Strands lying next to each other. Like radial roughness.

![](../.gitbook/assets/image%20%2891%29.png)

EEVEE doesn't support the Hair BSDF at all.

It works for the Principled BSDF though.

**The Principled Hair BSDF**

Mixed the Reflection and Transmission in a more physically accurate way \(based on shading model like Frozen and Zootopia!\).

**Melanin Concentration** gives realistic hair colors.

Use the **ColorRamp** node to control the darker and lighter area of the hair color.

![](../.gitbook/assets/image%20%2892%29.png)

\*\*\*\*



