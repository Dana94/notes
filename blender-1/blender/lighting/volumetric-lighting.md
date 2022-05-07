# Volumetric Lighting

In world view properties > volume > volume scatter with 0.1 density. This is with an HDRI selected already.

![](<../../../.gitbook/assets/image (137).png>)

Initially, the render will be completely black because the world view is set to be far away.

There needs to be lights within the scene to do this.

Have the point light outside of the scene in the same lane where the light is coming into the room.\
Pont: 25w, .05m in size.\
Under render > color management: exposure: 1.290.\
This will create a cool effect of a projector.\
\
<img src="../../../.gitbook/assets/image (141).png" alt="" data-size="original">

You can change the brightness by changing the amount of light bouncing by increasing the Light Paths > Max Bounces > Volume value. This determines how much light is bounces around in the room. Don't put the value higher than 2 or 3 for a brighter effect. Otherwise, there'd be too much noise in the render.

![](<../../../.gitbook/assets/image (143).png>)
