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

## Lightning:
- object data properties (in the shape of bulb) - change the color of the light , power-- 5000W, other options are sun, spot, area
- Tricks Shift + D for getting another light (press yellow dot to move it around)

<img width="784" alt="Screenshot 2023-10-13 at 5 27 40 PM" src="https://github.com/andysingal/AI-game/assets/20493493/56c92824-cb4b-4425-b89c-d8b318e25dd4">

## Editing Objects
- Shift +select + Press G to move the vertices of the object
<img width="950" alt="Screenshot 2023-10-18 at 6 56 03 PM" src="https://github.com/andysingal/AI-game/assets/20493493/05ef51f7-5de3-4706-a4fc-6dd5d4c877e2">
- Press the last one from above pic + press E to extrude
<img width="942" alt="Screenshot 2023-10-18 at 6 58 48 PM" src="https://github.com/andysingal/AI-game/assets/20493493/7beb6e6f-99fd-4961-89aa-5ec8485350b0">

Tips: Use Ctrl + R

<img width="567" alt="Screenshot 2023-10-18 at 7 35 17 PM" src="https://github.com/andysingal/AI-game/assets/20493493/86e444f0-a855-44b7-8a40-b8e7d03ea206">
- <strong>To move the object 20 steps g + Y + 20 </strong>

Tips: Move to a new collection by pressing M, Shift + A to add objects 
- view - Frame selected
- Insert face.. instead of E and S for resizing use Inset Faces
- E for entruding , Size for Sizing and then press 0 for pointy top 

<img width="137" alt="Screenshot 2023-10-18 at 10 59 12 PM" src="https://github.com/andysingal/AI-game/assets/20493493/dada5b15-8e38-4c64-8f7c-257bdf59d982">

Make the Rocky Base:
Create plane and Ico sphere and then go to Sculpting -- check Sculpt Mode 

Click on Dyntopo and press ok

<img width="364" alt="Screenshot 2023-10-25 at 7 24 20 PM" src="https://github.com/andysingal/AI-game/assets/20493493/d1736a58-8891-44d6-980f-7a95564027af">
- change the relative detail /constant detail 

Try the grab brush 

### Decimate Modifier 
1. goto Layout ---> Object Mode -->< Decimate Modifier -- Modify the Ratio 
<img width="383" alt="Screenshot 2023-11-01 at 8 52 41 PM" src="https://github.com/andysingal/AI-game/assets/20493493/c3cc06e1-8a2f-4d3d-87fb-bfc8087c693c">

Check the staistics:
<img width="325" alt="Screenshot 2023-11-01 at 9 12 11 PM" src="https://github.com/andysingal/AI-game/assets/20493493/05c7be41-6bf8-4f11-b6a4-513020aaf93f">



References:
- https://www.artstation.com/blogs/jsabbott/88mv/how-to-get-started-3d-modeling-in-blender-part-1-quick-start-guide
- https://www.creativebloq.com/3d-tips/blender-tutorials-1232739
