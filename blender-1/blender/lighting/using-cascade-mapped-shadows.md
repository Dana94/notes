# Using Cascade Mapped Shadows

Sun lamps use cascade shadows instead of cube mapped shadows.

Chang the sun value to 1000 and set the exposure to -7.8.

If under render > shadows you change the cascade size to a lower pixel, you'll get blocky shadows.

This is view dependent. How crisp the shadows are depends how zoomed in you are.

Under light > turn off contact shadows and set cascade shadow map count to 1 to see the same view no matter how zoomed in you are. The default 4 usually works well.

Fade is how much it transitions between the two. Set it to 0 will have it as a straight transition. Default is .1 which is fine.

Max distance set to 50 won't show any shadows zoomed out at all. It can e set to the distance of your camera in the scene.

Distribution is how close camera needs to be to get that highest resolution. Low value switches more when farther out. Opposite when its a higher value.&#x20;

Contact shadows work with point, spot, area lights.

Fix jagged shadow edges in render > shadows > toggle soft shadows on. Or rotate the light so it's not at an extreme angle.

Light threshold value is the same as custom distance value under a point light setting expect it's for all lights and calculated. It will cut off all lights after a certain distance.

