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

After choosing one of those option, you could brighten up the room using the world tab > ambient occlusion and change distance to something smaller than the size of the room like 10 feet. You can change the actor but that leaves everything a bit grey so instead create an area light outside the window. This adds extra light coming in though outside.

![](<../../../.gitbook/assets/image (146).png>)

Angle the area lamp down so it mimics sun light. Set strength to 250w with a color like the sky (pale blue).

When rendering this you can set the render sampling to 50 which is less detailed but less time to render while testing.

![](<../../../.gitbook/assets/image (147).png>)

Like before, with the sun only lighting the whole scene changing the sun strength or exposure didn't make a difference, they both gave similar results. If there are more light sources int he scene, it does change things.

Let's add lamps with light sources (despite this is a day scene) with each lamp shade containing a point light.

Add the first one with size .13 feet. Add a warm color. With power of 7w.

For the second one, hold down alt + D to create a "linked duplicate" which means whatever values you change for the first lamp point will also affect the second one.

![](<../../../.gitbook/assets/image (145).png>)

Now with more than 1 type of light in the scene, it rally matters on the differences of the types of lights. The sun is not bight enough compared to the lamps. If you change the sun angle value in the settings to 5 or 10 degrees it would make it believable.

Instead, remove this changed angle back to the default and change sun strength to 600. This will make it brighter in comparison to the lamps.

The range of the sun strength can be from 250 to 1100 depending on cloud conditions or type of day.

So this will have more light to bounce around the room. We can hide the area light in the render and viewport now to see the change. The bounce light from the sun will be much more natural.

The sun can be set to a more realistic color with a kelvin value. Change the HSV's S color to 0 (white). Under nodes > use nodes. Under color >  blackbody. Temperature is 5250.

Kelvin values can be found online.

The point lamps can have kelvin values too: 2700. (Following the saturation change, blackbody choice as well like the sun has.)

![](<../../../.gitbook/assets/image (143).png>)

Under shader editor > world with strength set to 200.\
This was through trial and error and comparing to real-world values.

Now the light from the sky illuminates the room better. No need for the area light trick anymore.

![](<../../../.gitbook/assets/image (141).png>)

If it looks too overexposed, render > color management decrease exposure to about -2.

You can lower exposure for sunlight to make the room darker or increase exposure for the lamps.

&#x20;![](<../../../.gitbook/assets/image (140).png>)

Yo can hit F11 to have the render window open and choose a new slot before hitting F12 to render the image. Don't compare images by changing slots because the exposure value will affect the previous slot too. Best to save the image and compare after.





