# Default 2D Animation

Best to rename the **object and the data** name the same.

![](../../../.gitbook/assets/image%20%28103%29.png)

Selecting the data bae is where you'll see the layers listed. The layer currently have mask, lock, hide, onion shown in that order for each layer.

![](../../../.gitbook/assets/image%20%28100%29.png)

Since we're switching form edit, object, and draw often, I checked "Tab for pie menu" so I could access them easier. Otherwise, they are at the top left of the interface under a dropdown.

![](../../../.gitbook/assets/image%20%28101%29.png)

When roughing out a sketch and you think it looks good, you can jump into the next frame in the same layer to finalize your drawing. Here, I'm going over my rough drawing in frame 2.

![](../../../.gitbook/assets/image%20%28104%29.png)

You may not need to fix the current rough sketch, so you could chose to move onto the lines layer in the same frame that the rough is in \(**so same frame, but different layer**\). Best to lighten the opacity for the rough one in this case. The rough layer's opacity isn't visible here but this is where it's adjusted.

![](../../../.gitbook/assets/image%20%28102%29.png)

Like for sculpting, **F** is for brush size, **shift + F** is for strength size.

Stabilize settings are under Options.

![](../../../.gitbook/assets/image%20%28109%29.png)

If using the stabilizer, there may be more vertices in your lines than necessary. Use Stroke &gt; Simplify to reduce these points. [Simplify Help](https://docs.blender.org/manual/en/latest/grease_pencil/modes/edit/stroke_menu.html#simplify)

Holding down shift reverses the stabilizer affect when you're drawing.

![](../../../.gitbook/assets/image%20%28110%29.png)

Best to autolock all layers you're not currently on.

![](../../../.gitbook/assets/image%20%28111%29.png)

Delete loose points option.

![](../../../.gitbook/assets/image%20%28107%29.png)

Each material has a stroke and a fill option.

![](../../../.gitbook/assets/image%20%28108%29.png)

Using the fill tool, you could see the boundaries it will fill before even adding the color in.

![](../../../.gitbook/assets/image%20%28106%29.png)

The sculpt brush can push the color into the right spot. Hit the alt key while using fill tool to create a boundary if the lines don't always create the desired boundaries for you.



If you are using the fill tool on a object with no complete boundary line, use Alt + LMB with fill enabled and the material has stoke checked. You will see a simple line drawn but it's used to encompass the color when you use fill. When you're done with the boundary, use edit mode &gt; grease pencil &gt; clean up &gt; boundary strokes.



If you want a selection of stroked to go behind others in the same layer, you can go to stroke &gt; arrange strokes &gt; send to back. This helps if the wrong colors are overlapping.

![](../../../.gitbook/assets/image%20%28105%29.png)

Use the mask layer option on the layer to clamp the shadows to the object only.

![](../../../.gitbook/assets/image%20%28112%29.png)

![](../../../.gitbook/assets/image%20%28120%29.png)

You can assign a material in edit mode with stroke &gt; assign material &gt; material in your collection.

![](../../../.gitbook/assets/image%20%28113%29.png)

Adding armature in Object mode shift + A &gt; Armature &gt; Single Bone \(in my version, it's only Armature as an option\).

Name the rig accordingly.

![](../../../.gitbook/assets/image%20%28121%29.png)

Rename the bone too.

![](../../../.gitbook/assets/image%20%28118%29.png)

In edit mode, grab the armature and position it to where the arm is.

![](../../../.gitbook/assets/image%20%28123%29.png)

When the first one is in its spot, hit E on the end to extrude it so another armature connects for the hand.

![](../../../.gitbook/assets/image%20%28117%29.png)

The second one is renamed too.

![](../../../.gitbook/assets/image%20%28119%29.png)

Constrain Melvin to armature with selecting it first then the armature and crtl + p to choose "with empty groups".

![](../../../.gitbook/assets/image%20%28122%29.png)

Now the vertex groups are available under Melvin.

![](../../../.gitbook/assets/image%20%28115%29.png)

In edit mode, choose what points are constrained to arm\_01 and hit assign. Do the same to the points for arm\_02.

![](../../../.gitbook/assets/image%20%28125%29.png)

Check the movement be something the armature in object mode and choosing pose mode. Select the top point and hit r to rotate.

![](../../../.gitbook/assets/image%20%28116%29.png)

For manipulating the armature:

edit mode for adjusting it

pose mode for testing it.

----

When it comes to keyframes, you cannot move them if they are locked.

![](../../../.gitbook/assets/image%20%28129%29.png)

Start animating in dope sheet when the bone is selected for pose mode.

![](../../../.gitbook/assets/image%20%28127%29.png)

Change bone display to B-Bone so it looks like 2 rectangles.

![](../../../.gitbook/assets/image%20%28128%29.png)

With the first bone part selected, choose 32 segments, then in edit mode, uncheck connected.

![](../../../.gitbook/assets/image%20%28126%29.png)

Select both bones on pose mode and hit I to insert a rotation key. \[couldn't see this option\]

A change in the waving arm was added in a keyframe every 4th sec.

![](../../../.gitbook/assets/image%20%28132%29.png)

To create the bend curve in the arm, change the Curve In Y value to -0.2 and the Curve out y value to -0.2. When the values are added, hit I over each one so they turn yellow. You may need to make sure the key frames before and after are set to 0 so it keeps the midway point.

![](../../../.gitbook/assets/image%20%28131%29.png)



