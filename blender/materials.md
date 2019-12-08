---
description: 'A bit messy right now, just jotting down what comes to mind.'
---

# Materials

When first opening the node editor for materials, it can seem pretty daunting \(I still feel this way\).

Considering when applying materials for an object. What are all the different surfaces you are trying to show on the object?

Is it scuffed? Polished? Wooden? Plastic? Glass?

Knowing what you are trying to achieve with the final render can guide you through creating the materials.

Metallic - underlying surface \(gives a shiny appearance\)

Diffuse - paint color \(default material, solid color overall\)

Reflective - Paint finish \(how much the object material reflects its surroundings\)

Texture - Grime and scratches \(Images \(like png\) that can give the object a specific appearance through scratches and grime. Textures can allow materials underneath to show through.\)



Within the node editor, you can group panels by selecting one or more \(use shift for many\) and select Layout &gt; Frame to place it on the nodes you want to capture.

You can rename the panel by selecting it and entering n to open the menu. Edit the label input and you'll see your change when you hit enter.

If you want to directly attach a node to the Material Output, hit shift  + ctrl + click on the node.

Hit M to mute a node. This will keep a node from affecting the material. Hit M again to unmute it.



Diffuse + Glossy

Mix Shader \( .5 / .5 \) --&gt; Shiny plastic

Mix Shader \( .5 / .1 \) --&gt; Realistic plastic



Input &gt; Fresnel

A range where you can change the reflective amount. By default, it will show the mesh all black, then transforming into white along the edges the farthest away from you. Facing us is the darkest reflection \(less reflection\).

Fresnel removes equal reflection everywhere.

Helps with intensity of reflection and roughness of reflection.



Converter &gt; Color Ramp

By using Fresnel as an input, color ramp can give a value for roughness \(like on Glossy BSDF\) if a Power \(default .5\) is assigned between them.

Set Black to .001 for RGB since absolute black is too intense.

Set White to .05 for RGB for whatever value is the minimum set for, say, the Glossy BDSF roughness.

What's weird is that the color output from color ramp goes into the left value for Power. The Power's right value output goes into Glossy's rough value input. I thought the input/output colors determined what values could be used for other inputs/outputs.



Anisotropic BSDF

Anisotropy - Gives a brushed metal effect. This value changes the rotation of reflection \(stretches the metal\). If you set this value to 0, it will have the same affect as Glossy BSDF, so it wouldn't make sense to keep it at 0. 



Image Texture

Upload an image to incorporate into the material. It can mapped to specific regions of the object so specific colors are in predetermined places on the mesh.

Set this to non-color data.



Normal Map

Can be used to help place an image texture properly on the mesh. This may not be necessary, depending on the state of the image texture.

Its output can be connected to various inputs at the same time.





