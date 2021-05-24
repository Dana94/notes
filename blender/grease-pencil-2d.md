# Grease Pencil \(2D\)

Credit to this [video](https://www.blendernation.com/2021/02/20/how-to-render-a-grease-pencil-animation-video-basic-settings-blender-2-9/).



**Render &gt; Render Animation** to render your animation.



First! Check our output properties before rendering.

![](../.gitbook/assets/image%20%2895%29.png)

**Resolution x and y** are camera dimensions.

**Frame Start and End** depends on when your animation frame ends at.



Select what media type is exported.

![](../.gitbook/assets/image%20%2897%29.png)



Choosing PNG would render an image for every frame and put them in the folder you selected.

AVI JPEG is a compressed video format.

AVI Raw is a compressed format.

FFmpeg video is .mp4 format for uploading.



Encoding Properties

![](../.gitbook/assets/image%20%2894%29.png)

Data container is data extension. MPEG-4 is common for cross platform use.

Video Codec is for video compression. H.264 is default and recommended.

Audio Codec needs to be defined if there is audio present.





Render Properties Transparent Background

![](../.gitbook/assets/image%20%2898%29.png)

Cannot render an animation with transparent bg but you can render separate images for each frame with a transparent background option checked and put them together with a video making software.

If you choose this path, make sure the Color option under Output is RGBA.

For a grease pencil animation, the render settings can be smaller.

![](../.gitbook/assets/image%20%2896%29.png)



