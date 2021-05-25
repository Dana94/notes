# The Principled Shader

**Subsurface**: Increasing size in subsurface scattering node.

**Subsurface Radius**: Control which wavelengths of light make it farther through our object.

**Subsurface Color**: The color underneath the top layer.

**Metallic**: Usually 0 or 1. Can add an image texture for this.

**Specular**: Controls reflectivity or Fresnel.

**Specular Tint**: Don't use with a colored-nonmetal. Used to tint reflections.

**Roughness**: Can use an image texture for.

**Antistrophic**: Higher roughness will pull reflections along a particular line.

**Sheen**: Mixing in Bevel with Diffuse material. Good for soft materials with tiny hairs to catch the light.

**Sheen Tint**: Same as Specular Tint but for Sheen.

**Clearcoat**: Second Glossy shader. Highly reflective layer coat.

**Transmission**: Gives Glass affect. Set IOR: 1 will give a transparent material.

**Transmission Roughness**: Roughness of the refraction.

**Emission**: Emit colored light with Specular to 0.

Does not have translucency to allow light to pass straight through.

![](../../.gitbook/assets/image%20%2890%29.png)

