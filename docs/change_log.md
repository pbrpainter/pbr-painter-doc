# Changelog
_Please note that by purchasing PBR Painter you will have access to every update that is released, indefinitely and for no extra cost._

The below shows the _major_ changes made to the addon over previous versions. Note that not all _minor_ changes are mentioned.

- __v2.3.1:__
	- Minor bug fixes
	- Ported for added compatibility with Blender 3.2 (still backwards compatible with earlier versions)

- __v2.3:__
	- Add a new ID map system with multiple colors
	- Modify material slots UI to automatically determine when to be in texture paint mode when selecting a material
	- Move addon outside of texture paint mode to open up access to new features
	- Develop a dedicated workspace layout for PBR Painter
	- Add preview option for each layer, rather than just when using procedural textures
	- Add filled layer option, removing the need to fill every layer (painted layers as you know them will still remain!)
	- Create a new setup for painted layers, giving easier access to the built-in painted mask via the mask stack
	- Add option to ignore layer's masks for a given channel
	- Replace single channel layers with the option to paint over image textures in multichannel layers
	- Restructure the UI to give easy access to the main channels (color, roughness, metallic etc)
	- Add option to use another layer's mask in the current layer's mask stack
	- Add option to use different UV maps for textures, masks etc
	- Add option to bake textures and masks to a different UV map
	- Add option to import a layer, or all layers, from another material
	- Add option to import a mask, or all masks, from another material
	- Integrate with 3.0 asset browser, to allow for saving and loading smart materials, layers, masks etc. (still to be added to/improved upon in future
	- Add option to use node group as a mask
	- Add new icons etc. to improve the overall appearance and user-friendliness of the addon
	- Add ambient occlusion option during baking 
	- Add options to use different edge detection methods for preset edge wear masks
	- Add vertex color option for ID maps
	- Add new "View Mode" option, accessible via the three dots button next to the layer stack. You can now select either Material (which is the standard view) or Single Channel. 
	- Added vertex color as an option for ID map, with the Fill Selected Faces feature. This will fill the selected faces with the vertex color that is selected (very useful for quickly creating ID maps for materials).
	- Add the option to create an Exportable Material when baking. This will setup a new material (or use a material from a dropdown menu) with the baked textures, ready to export via 

- __v2.2:__
	- Improved addon performance by automatically cleaning up unused images and node groups associated with deleted layers
	- Added option to bake and/or merge all PBR Painter materials on mesh to single texture set
	- Revamped mask system to enable layer masks on custom layers and imported material layers
	- Improved overall addon efficiency and performance
	- Streamlined UI for brush settings
	- Added extra procedural options
	- Added buttons for preset texture resolution (1k, 2k etc)
	- Added drop down for mapping mode (point vs texture)
	- Added option to import a material node setup as a layer 
	- Added option to adjust color settings for albedo textures (hue/saturation and RGB curves)
	- Streamlined access to other materials in the model's material slots
	- Improved background layers to be more streamlined, efficient and easy to use
	- Fixed a few minor bugs with importing materials
	- Fixed a bug causing ID maps to sometimes not turn off correctly
	- Added a preset "Edge Wear" mask
	- Added a few new options to different parts of the UI (e.g. option to have new layer auto-filled, option to change merged mask name etc.)
	- Added color ramp to Normal channel when using a bump map
	- Fixed a bug causing multi-texture import to fail for "glossiness" textures
	- Fixed a few bugs with baking
	- Fixed a bug with the new box mapping rotation system (normals were being calculated globally rather than locally, which was causing the box mapped textures to change when the object was rotated)
- __v2.1:__
	- Introduced option to instantly import and assign a set of textures automatically
	- Introduced option to instantly link multiple channels to the layer mask automatically and simultaneously, speeding up the procedural workflow
	- Introduced new addon preferences (autosave now in addon preferences)
	- Moved background layer panel to more discrete button in UI
	- Introduced additional mapping options for masks
	- Introduced a mask multiplier for each channel, for finer control over channel masking
	- Introduced a range of preset procedural mask options (currently scratches, grunge and cracks, more to be added), which are tunable and can be incorporated into the mask stack
	- Improved UI by adding visual cues showing which channels are switched on/off in a layer
	- Improved texture importing
	- Overhauled baking system for performance improvement and a smoother user experience.
	- Minor bug fixes relating to baking textures.
	- Added option to use relative or absolute texture paths in PBR Painter (located under addon preferences).
	- Fixed bug causing an error during unregistering, and causing the clearcoat and clearcoat roughness panels to be hidden.
	- Some minor bug fixes
	- Added option to overwrite previously baked textures during baking
	- Changed naming convention for merged textures for clarity
- __v2.0:__
	- Major overhaul of addon for a huge boost to performance
	- Restructured UI for a more intuitive, more user-friendly and less busy interface
	- New option for importing a height/bump map in the normal channel
	- Brand new masking system, using layered system to build complex and highly-specific masks
	- More options for each specific mask (which can individually be added to the layered setup)
	- New displacement threshold mask, which applies a mask according to the displacement of previous layers (very cool!)
	- New option to use a custom layer, which lets you build your own layer from scratch using your own node setups, which can then be painted as a layer as per normal (important for advanced users who need highly specific node setups)
	- New copy/paste functions for procedural texture setups, for copying between channels and/or between layers
	- Improved how deleted layers are stored for improved addon performance and efficiency
	- New automated external texture saving after baking using a user-defined file directory
	- Fixed a bug with the autosave feature which was causing it to not save when the mouse was over the 3D viewport.
	- Added option to set the time between autosaves
	- Fixed a bug with duplicate mask
	- Fixed a bug that was occasionally causing an error when using a custom brush
	- Fixed a bug with the specular tint channel when using link to mask
	- Fixed a bug when using merge masks that was causing the active image to switch away from the painted mask for the layer
	- Fixed a bug when duplicating an alpha map mask with box mapping selected
	- Additional bug fixes related to normal baking
	- Added the option to boost the strength of baked normal textures, which can be used to add stronger details or if the baking is producing maps that are too weak
	- Fixed a bug that was sometimes causing an error after deleting then restoring a layer containing masks
	- Fixed a bug with external texture baking that was sometimes causing the color space of saved textures to be incorrect
- __v1.1:__
	- New option to paint a procedural texture for each separate PBR channel (noise, voronoi, musgrave or wave), with tools to tune/scale/rotate these as necessary
	- Additional mask options (procedural noise, voronoi, musgrave or wave) that can be used in combination with all currently available masks
	- New autosave feature which, when turned on, automatically saves modified textures periodically, to avoid accidentally losing work
	- New duplicate layer button
	- Optional color ramp node when using a roughness, specular or metallic texture, for fine-tuning the texture (e.g. make a roughness texture more glossy)
	- Box mapping now available for imported textures, with access to a seam blend slider for creating seamless materials
	- New bake button to be used for baking the current material textures without having to use the merge visible button
	- Improved naming of baked textures to be more specific and streamlined
	- Option to adjust normal strength for each layer individually
	- Bump mapping available as an option in single pass layers
	- New button to instantly invert any color ramp in the addon.
	- Fixed bug that was occasionally causing an error when switching between paint and erase, or when adding a layer
	- Introduced the option to change the blend type between layers, for each channel in a layer
	- Reduced dependency on internal operations for better compatibility with future Blender versions
- __v1.0:__ 
	- Release version
