# UV Editing

## Unwrapping mesh

Example:

Add a Torus object and then go into UV Editing tab.

![](../.gitbook/assets/image%20%288%29.png)

On the left, you'll see a grid which is where the unwrapped mesh object will appear.

Go into edit mode and have the whole mesh selected.

![](../.gitbook/assets/image%20%2814%29.png)

You'll see a mesh unwrapped on the object on the left side. This is a default unwrap. I'll show you in the next step, how to unwrap the mesh in a more specific way.

Hit **a** twice to deselect the mesh, then hit **shift + alt while selecting** the center line going around the torus.

![](../.gitbook/assets/image%20%2811%29.png)

Ctrl + E &gt; Mark Seam to create a seam on the selected line.

![](../.gitbook/assets/image%20%2829%29.png)

You should see a red line on what you marked as a seam.

![](../.gitbook/assets/image%20%282%29.png)

Now select the whole mesh again, then hit **u &gt; Unwrap** to see a new unwrap show in the left panel.

![](../.gitbook/assets/image%20%2839%29.png)

![](../.gitbook/assets/image%20%2834%29.png)

Well that looks different! When you mark a seam, it indicates where the program should "cut" along in order to create a different unwrapping.

Here's an explanation showing where the scissors would be cutting the mesh and how the sides would flip in order to produce the new UV layout.

![](../.gitbook/assets/image%20%2841%29.png)





