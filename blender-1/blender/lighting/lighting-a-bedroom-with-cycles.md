# Lighting a Bedroom with Cycles

Best to have a dedicated workspace for lighting our project. Just duplicate the Layout tab at the top and rename it "Lighting".

Use a sun light to cast light on the area in your scene you want the eyes to focus on.

Change the strength of the lamp to 15w which is more realistic to what a sunlamp would be.

Make sure that under render > color management > view transform value is Filmic.

Change sun color to a warmer color (pale orange or something) like what the sun would be.

Under world tab choose a sky texture under color value > sky texture.

Change strength of this texture to 50 to make it more realistic. This is determined by playing with it.\
Right now, this isn't really realistic to a daylight scene. The room isn't illuminated as much as is expected.

![](<../../../.gitbook/assets/image (139).png>)

Checking under render > light paths, the value of diffuse is 16 which should be enough.

2 things to fix this, either increase the strength of the sun or change the exposure.

Since the sun lamp (and a bit of the sky texture) is the only light source, it doesn't really matter which one you choose.

* Change the exposure to about 4 will blow up the light and make it more realistic. If the render is too noisy, just up the sampling > viewport to 50.
* If not changing exposure, increase sun strength to 50 and notice the light bounce around the room.

After choosing on e of those option, you could brighten up the room using the world tab > ambient occlusion and change distance to something smaller than the size of the room like 10 feet. You can change the actor but that leaves everything a bit grey so instead create an area light outside the window. This adds extra light coming in though outside.

