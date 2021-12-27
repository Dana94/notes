# Default 2D Animation

Best to rename the **object and the data** name the same.

![](<../../../.gitbook/assets/image (103).png>)

Selecting the data bae is where you'll see the layers listed. The layer currently have mask, lock, hide, onion shown in that order for each layer.

![](<../../../.gitbook/assets/image (100).png>)

Since we're switching form edit, object, and draw often, I checked "Tab for pie menu" so I could access them easier. Otherwise, they are at the top left of the interface under a dropdown.

![](<../../../.gitbook/assets/image (101).png>)

When roughing out a sketch and you think it looks good, you can jump into the next frame in the same layer to finalize your drawing. Here, I'm going over my rough drawing in frame 2.

![](<../../../.gitbook/assets/image (104).png>)

You may not need to fix the current rough sketch, so you could chose to move onto the lines layer in the same frame that the rough is in (**so same frame, but different layer**). Best to lighten the opacity for the rough one in this case. The rough layer's opacity isn't visible here but this is where it's adjusted.

![](<../../../.gitbook/assets/image (102).png>)

Like for sculpting, **F** is for brush size, **shift + F** is for strength size.

Stabilize settings are under Options.

![](<../../../.gitbook/assets/image (109).png>)

If using the stabilizer, there may be more vertices in your lines than necessary. Use Stroke > Simplify to reduce these points. [Simplify Help](https://docs.blender.org/manual/en/latest/grease\_pencil/modes/edit/stroke\_menu.html#simplify)

Holding down shift reverses the stabilizer affect when you're drawing.

![](<../../../.gitbook/assets/image (110).png>)

Best to autolock all layers you're not currently on.

![](<../../../.gitbook/assets/image (111).png>)

Delete loose points option.

![](<../../../.gitbook/assets/image (107).png>)

Each material has a stroke and a fill option.

![](<../../../.gitbook/assets/image (108).png>)

Using the fill tool, you could see the boundaries it will fill before even adding the color in.

![](<../../../.gitbook/assets/image (106).png>)

The sculpt brush can push the color into the right spot. Hit the alt key while using fill tool to create a boundary if the lines don't always create the desired boundaries for you.



If you are using the fill tool on a object with no complete boundary line, use Alt + LMB with fill enabled and the material has stoke checked. You will see a simple line drawn but it's used to encompass the color when you use fill. When you're done with the boundary, use edit mode > grease pencil > clean up > boundary strokes.



If you want a selection of stroked to go behind others in the same layer, you can go to stroke > arrange strokes > send to back. This helps if the wrong colors are overlapping.

![](<../../../.gitbook/assets/image (105).png>)

Use the mask layer option on the layer to clamp the shadows to the object only.

![](<../../../.gitbook/assets/image (112).png>)

![](<../../../.gitbook/assets/image (120).png>)

You can assign a material in edit mode with stroke > assign material > material in your collection.

![](<../../../.gitbook/assets/image (113).png>)

Adding armature in Object mode shift + A > Armature > Single Bone (in my version, it's only Armature as an option).

Name the rig accordingly.

![](<../../../.gitbook/assets/image (121).png>)

Rename the bone too.

![](<../../../.gitbook/assets/image (118).png>)

In edit mode, grab the armature and position it to where the arm is.

![](<../../../.gitbook/assets/image (123).png>)

When the first one is in its spot, hit E on the end to extrude it so another armature connects for the hand.

![](<../../../.gitbook/assets/image (117).png>)

The second one is renamed too.

![](<../../../.gitbook/assets/image (119).png>)

Constrain Melvin to armature with selecting it first then the armature and crtl + p to choose "with empty groups".

![](<../../../.gitbook/assets/image (122).png>)

Now the vertex groups are available under Melvin.

![](<../../../.gitbook/assets/image (115).png>)

In edit mode, choose what points are constrained to arm\_01 and hit assign. Do the same to the points for arm\_02.

![](<../../../.gitbook/assets/image (125).png>)

Check the movement be something the armature in object mode and choosing pose mode. Select the top point and hit r to rotate.

![](<../../../.gitbook/assets/image (116).png>)

For manipulating the armature:

edit mode for adjusting it

pose mode for testing it.

\----

When it comes to keyframes, you cannot move them if they are locked.

![](<../../../.gitbook/assets/image (129).png>)

Start animating in dope sheet when the bone is selected for pose mode.

![](<../../../.gitbook/assets/image (127).png>)

Change bone display to B-Bone so it looks like 2 rectangles.

![](<../../../.gitbook/assets/image (128).png>)

With the first bone part selected, choose 32 segments, then in edit mode, uncheck connected.

![](<../../../.gitbook/assets/image (126).png>)

Select both bones on pose mode and hit I to insert a rotation key. \[couldn't see this option]

A change in the waving arm was added in a keyframe every 4th sec.

![](<../../../.gitbook/assets/image (132).png>)

To create the bend curve in the arm, change the Curve In Y value to -0.2 and the Curve out y value to -0.2. When the values are added, hit I over each one so they turn yellow. You may need to make sure the key frames before and after are set to 0 so it keeps the midway point.

![](<../../../.gitbook/assets/image (131).png>)

Toggle overlays to hide the armature.

![](<../../../.gitbook/assets/image (133).png>)



Tips:

* If you don't see anything in your dope sheet, highlight the armatures.
* If the armatures aren't showing toggle overlays OR check the scene collection if they are marked as hidden.

Make sure to turn off auto keying when you're done.

![](<../../../.gitbook/assets/image (135).png>)



Create a background in object mode using shift + a > grease pencil > blank.

Use the draw tool to create a square around the camera view. Hit enter to confirm.

![](<../../../.gitbook/assets/image (136).png>)

If you see our background but not the object, it's probably because they are in the same place and the background object needs to be moved behind it.

![](<../../../.gitbook/assets/image (134).png>)
