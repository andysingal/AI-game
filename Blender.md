- edit > preferences > emulated numpad: The Numpad keys are used quite often in Blender and are not assigned to the same action as the regular number keys. If you have a keyboard without a Numpad (e.g. on a laptop), you can tell Blender to treat the standard number keys as Numpad keys by checking Emulate Numpad
- press 1 for front view and 7 for top view 
- Add> Mesh>Cube 

## Adding Objects: 
Cursor to Selected: SHIFT+S
-N for short cuts

If you use “Cursor to selected” while in object mode, then the 3D cursor will move to the selected objects origin point. You can also use Cursor to selected in other modes such as edit mode

- press G to move along x-axis
- press y to move along y-axis
-  press R for rotation
-  move light:
  1. Select the light in the viewport by left clicking on it - it should be highlighted in yellow.
  2. press g, then move your mouse to move the object. If you want to move it along a specific axis, you can press g, and then press, for example, x, to move it along the x axis.


## ViewPort and Rendering
- Using Viewport shading for Wireframe
Shadown Workspace:
- Camera and you get Rander properties
-  Render Engine - Render properties -- Eevee/Cycles
   - Move your camera to a position where you can see all your objects
   - Move your light into a nice position

Togle to camera view -- > press N -- Lock--Camera to View

## Material Colors:
- Select the objection, in the bottom window select New -> Base Color(Saturation) followed by Hue, Value for coloring the object
- You can select other objects to keep the same color 

<img width="1536" alt="Screenshot 2023-10-13 at 2 03 51 PM" src="https://github.com/andysingal/AI-game/assets/20493493/7e240d3c-2ad1-43ae-93ba-cf53aea62ecc">
- Press N and below Render Engine:  

check [Ambient Occlusion](https://docs.blender.org/manual/en/latest/render/eevee/render_settings/ambient_occlusion.html)

or Check [Screen Space Reflections](https://docs.blender.org/manual/en/latest/render/eevee/render_settings/screen_space_reflections.html)

Further Render Image:

![Rendered Image](https://github.com/andysingal/AI-game/assets/20493493/663f0233-eaa6-4784-8b16-17bcccd5d50f)

## Material Reflections

- Further we will be changing the Metallic, Roughness and Normal in the principled BSDF (metallic..1.0, no roughness)
- Right click on the object and select shade smooth 
- Further click on object data properties --> Normal-- Auto Smooth
- To further improve reflection, object-> world

<img width="1286" alt="Screenshot 2023-10-13 at 3 03 42 PM" src="https://github.com/andysingal/AI-game/assets/20493493/08b5e2b0-6b37-492d-bb22-5aca60e5d40f">
For adding images instead of color, go to https://polyhaven.com/
<img width="1047" alt="Screenshot 2023-10-13 at 3 36 31 PM" src="https://github.com/andysingal/AI-game/assets/20493493/00b11ec3-dca5-4e96-b9b2-7dc4d0dd9de1">

Lightning:
- 

References:
- https://www.artstation.com/blogs/jsabbott/88mv/how-to-get-started-3d-modeling-in-blender-part-1-quick-start-guide
- https://www.creativebloq.com/3d-tips/blender-tutorials-1232739
