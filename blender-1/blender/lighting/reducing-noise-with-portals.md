# Reducing Noise with Portals

Using HDRIs to light a scene can cause a lot of noise particles in your render. To only focus on the rays coming directly from the light source, you can use a portal of an area light.

Uncheck portal option for the area light and place it in the path of the window where the ray of light is entering. The size should be the same as the window size otherwise it would cause more calculating. This is best for smaller windows where it would have a much bigger effect.

![](<../../../.gitbook/assets/image (144) (1).png>)
