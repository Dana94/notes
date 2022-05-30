# Using Contact Shadows

Using rasterize shadows, you'll see that light still seeps through at the bottom of a plane eve through it's going through the floor.

![](<../../../.gitbook/assets/image (143).png>)

Toggling **contact shadows** on in the light setting fixes this.

![](<../../../.gitbook/assets/image (146).png>)

The distance value is determined by checking it fixes the crack of light but doesn't add too much extra in the corner. This can be fixed so it can just blend in with the shadow. I set it to around 0.8 here. Bias works the same way as the shadow bias, but for contact shadows specifically. The default value (.03) works generally well for use.

![](<../../../.gitbook/assets/image (145).png>)

Thickness value will help us reduce the protrusion of the shadow from the wall. Setting it too high will show a streak of shadow up the vertical side of the wall.

![](<../../../.gitbook/assets/image (138).png>)

If you ever come across an object not casting the right shadow or there's light leaking, you may need to make your geometry a bit thicker. In eevee, objects should have some thickness to avoid light leaks.

