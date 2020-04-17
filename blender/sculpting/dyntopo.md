---
description: Dynamic topology
---

# Dyntopo

Check box in top right of sculpting window.

![](../../.gitbook/assets/image%20%2829%29.png)

If you get an error when turning dyntopo on, remove the mesh object automatically created for you when adding a new object.

![](../../.gitbook/assets/image%20%2840%29.png)

The topology won't stretch and it is generated on the fly.

![](../../.gitbook/assets/image%20%2813%29.png)

### Settings

![](../../.gitbook/assets/image%20%2830%29.png)

Detail size: the more finer the detail, the higher the pixel size.

Refine Method:

* Subdefine collapse: will create new topology regardless of underlying topology
* Subdefine edges: 

Detailing: detail size is directly related to this.

* Constant - related to resolution. \(in blender units - the squares on the grid floor\)
* Brush - according got size of the brush
* manual - detail flood fill assigns the current topology over the entire mesh \(not really a good use if sculpting is meant to isolate the object when working on it\)

