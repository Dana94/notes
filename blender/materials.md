---
description: 'A bit messy right now, just jotting down what comes to mind.'
---

# Materials

Diffuse + Glossy

Mix Shader \( .5 / .5 \) 

--&gt; Shiny plastic



Within the node editor, you can group panels by selecting one or more \(use shift for many\) and select Layout &gt; Frame to place it on the nodes you want to capture.

You can rename the panel by selecting it and entering n to open the menu. Edit the label input and you'll see your change when you hit enter.



Input &gt; Fresnel

A range where you can change the reflective amount. By default, it will show the mesh all black, then transforming into white along the edges the farthest away from you. Facing us is the darkest reflection \(less reflection\).

Fresnel removes equal reflection everywhere.



Converter &gt; Color Ramp

By using Fresnel as an input, color ramp can give a value for roughness \(like on Glossy BSDF\) if a Power \(default .5\) is assigned between them.

Set Black to .001 for RGB since absolute black is too intense.

Set White to .05 for RGB for whatever value is the minimum set for, say, the Glossy BDSF roughness.

What's weird is that the color output from color ramp goes into the left value for Power. The Power's right value output goes into Glossy's rough value input. I thought the input/output colors determined what values could be used for other inputs/outputs.



