---
description: Used on point or spotlights.
---

# Texturing Lights with IES Data

IES - Illuminating Engineering Society

Under a light point setting, Nodes > choose nodes.\
In the shader view, create add node "IES Texture". Upload an external .ies file and adjust the strength to get some cool effects on the objects.

![](<../../../.gitbook/assets/image (138).png>)

This won't only simulate the light bulb, but the fixture that it's in. The light is a bit normalized, so it's best to grab a new point (or duplicate this one and remove the IES texture node and adjust the strength value until you like how it looks.) Then adjust the IES one to match it until you don't need the reference anymore.

