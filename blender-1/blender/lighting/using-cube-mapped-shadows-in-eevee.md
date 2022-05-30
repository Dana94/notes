# Using Cube Mapped Shadows In EEVEE

Biggest difference between eevee and cycles is how shadows interact with the scene.

Specular value in a light point has to do with the tiny bright ness in the center of a reflected light.

In cycles, good to have multiple lights with realistic values and set the exposure to make things brighter.

In eevee, with a realistic light point and the world strength set to .01. The light doesn't go very far.

\
![](<../../../.gitbook/assets/image (145) (1).png>)\


Set the point light to custom distance to fix this. Keep the distance small so less to calculate.\


![](<../../../.gitbook/assets/image (142).png>)



To disable "soft shadows" go under render tab > shadows > soft shadows.

Soft shadows can be defined by cube size values. It's created by 360 degree image (or a cube map) from this point in space.

![](<../../../.gitbook/assets/image (143) (1).png>)

Under light settings, shadow > clip start is the distance in which objects will start casting shadows.

If you have a shape covering a light source, it's best to make the clip start value bigger than the object covering it so the light can still be seen.



![](<../../../.gitbook/assets/image (144).png>)



The Bias value is so the smaller it is, the more tiny details are able to cast shadows. 0.1 is pretty good because if soft shadow is used, it will blend the small parts of shadow.
