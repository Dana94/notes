# Lighting a Bedroom with Cycles

Best to have a dedicated workspace for lighting our project. Just duplicate the Layout tab at the top and rename it "Lighting".

Use a sun light to cast light on the area in your scene you want the eyes to focus on.

Change the strength of the lamp to 15 which is more realistic to what a sunlamp would be.

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

After choosing one of those option, you could brighten up the room using the world tab > ambient occlusion and change distance to something smaller than the size of the room like 10 feet. You can change the factor but that leaves everything a bit grey so instead create an area light outside the window. This adds extra light coming in though outside.

![](<../../../.gitbook/assets/image (146) (1).png>)

Angle the area lamp down so it mimics sun light. Set strength to 250w with a color like the sky (pale blue).

When rendering this you can set the render sampling to 50 which is less detailed but less time to render while testing.

![](<../../../.gitbook/assets/image (147).png>)

Like before, with the sun only lighting the whole scene changing the sun strength or exposure didn't make a difference, they both gave similar results. If there are more light sources in the scene, it does change things.

Let's add lamps with light sources (despite this is a day scene) with each lamp shade containing a point light.

Add the first one with size .13 feet. Add a warm color. With power of 7w.

For the second one, hold down alt + D to create a "linked duplicate" which means whatever values you change for the first lamp point will also affect the second one.

![](<../../../.gitbook/assets/image (145) (1).png>)

Now with more than 1 type of light in the scene, it rally matters on the differences of the types of lights. The sun is not bright enough compared to the lamps. If you change the sun angle value in the settings to 5 or 10 degrees it would make it believable.

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

![](<../../../.gitbook/assets/image (141) (1).png>)

If it looks too overexposed, render > color management decrease exposure to about -2.

You can lower exposure for sunlight to make the room darker or increase exposure for the lamps.

&#x20;![](<../../../.gitbook/assets/image (140) (1).png>)

Yo can hit F11 to have the render window open and choose a new slot before hitting F12 to render the image. Don't compare images by changing slots because the exposure value will affect the previous slot too. Best to save the image and compare after.

The last way we can light the scene is with an HDRI without a sun in the sky.

Hide the 2 point lights and add an Environment Texture node in the world shader editor plugging it into the background node.

![](<../../../.gitbook/assets/image (144).png>)

Since we don't know how bright this should be, disconnect the background from the output node and with only the sun spot showing adjust the exposure to the value -3.977.

Then, hide the sun and connect the background node to the output again and adjust the strength there until it matches visually as the sun's effect. Since the sun isn't coming into the room, the HDRI needs to be rotated to get a pattern on the bed or wall.

Click on the HDRI node and hit "N" to open the sidebar.

Under texture mapping > rotate Z value should be changed to about -81.5 degrees so the light hits the pillows. Change the view transform value to "False Color" to see the light values from this light exposure. You can look back at the sun's effect by disconnecting the output node again and turning on the sun. To adjust the HDRI strength, change it to 150 for a more similar effect to the sun's.

Go back to "Filmic" and turn on the lamps. Make sure to disablet he sun for the render too.

Change the exposure for the inside with values (0-positive) or the outside (negative values).

We're trying to get a similar effect as the previous image using the sun point.

Choose a new slot after hitting F11 and then F12 to render.

A main advantage of using HDRI is that we get more natural colors in the bounce lighting.

A disadvantage that it could be slower to render or more noisy.

You could turn on the area light again and turn on "portal" in the light settings to clean up the noise a bit faster.

\-------------------

For a dark scene, change the HDRI with a dark sky. Rest the Exposure by clicking it and hitting backspace so it resets. Change the background strength in nodes to 1.

![](<../../../.gitbook/assets/image (141).png>)

Disconnect the background node from the world output so the render is completely black. Don't forget to uncheck ambient occlusion from the world view settings.

Now to add a sunlight to the strength of what the moon should be so we can set the HDRI to the correct strength. Copy the sun lamp in the scene with Shift + D and rename it as moon. Change the strength of the mon light in its settings to .001. The scene should still be in darkness. Turn up the exposure to its max (10) to see how the light affects the scene.

![](<../../../.gitbook/assets/image (146).png>)

Then hide the moon, and plug the background node back into the world output. Change the background node strength to .005 (had to play with this to find this as the best value).

Then turn on the lamp lights and move the exposure down to 3. You can also change the rotation of the HDRI again in the node editor.

![](<../../../.gitbook/assets/image (140).png>)

Since there's a noticeably big shaded error above the bed, we may wan to fix that since it's the center of the room. Hit Shift + D on the one of the lamp lights and move it to the middle of the ceiling. If it's too low, it will be reflected in the window which would looks strange. Change the exposure to 2.

Hide all lamps in the room (lamps and bedroom one) and add another point light copy in the hallway. Change power to 15 and temperature to 3500 so it's more of a LED type light.

![](<../../../.gitbook/assets/image (145).png>)

Turn the other 3 light sources on and render it out.

