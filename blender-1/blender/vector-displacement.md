# Vector Displacement

[Source](https://www.youtube.com/watch?v=ekaQPkEdudw)

To make vector displacement work, there needs to be a **subdivision surface modifier** on my object.

Then change the render engine to **Cycles** with the feature set as **Experimental**.

Then there will be an **adaptive subdivision** option to choose which gives you new options in the modifier.

![](<../../.gitbook/assets/image (137).png>)\


Within the shader editor, have the material output selected and change the surface displacement option to **Displacement and Bump**.

Then set the gradient texture and color ramp to the other nodes like this:

![](<../../.gitbook/assets/image (138).png>)
