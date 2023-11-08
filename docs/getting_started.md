# Getting Started

## Installation and Loading the PBR Painter Workspace

<p><iframe width="560" height="315" src="https://www.youtube.com/embed/mAGIwUKqm5E" title="YouTube video player" 
frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

When you purchase PBR Painter, you will have access to the .zip file that contains the entire addon package. 

This can be installed in Blender using the normal approach:
![Screenshot](img/installation.gif)

## Updating to New Versions

If you already have an old version of PBR Painter installed, and wish to update to a new version, please follow the following steps:
<p><li> 1. Completely uninstall the old version from Blender. </li>
<li> 2. Close and restart Blender to ensure any cached files are cleared. </li>
<li> 3. Install the new version as per normal. </li></p>

## Setting up the Asset Browser (Blender 3.x and 4.x Only)
<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/cpHb4JseF_U" title="YouTube video player" 
frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

If you are using Blender 3, it is recommended that you choose an asset directory, within the addon preferences. This will create a new filepath to tell Blender where
you're PBR Painter assets will be stored.

## Important Considerations (PLEASE READ)

There are a few things to consider before getting started as these will have a considerable impact on your experience with PBR Painter:

- PBR Painter generates complex node groups associated with each layer. These are created, modified, connected and deleted using the various
tools within the addon, so you never actually need to even look at the node tree. __It is important to NOT delete any of the node groups created
by PBR Painter as this could cause issues with the addon. Deleting nodes _within_ a node group may break the addon entirely.__

- There is a limit on the number of image texture nodes that can be represented using __Eevee__ (and also for __Cycles__, but it is much higher). If you reach this limit 
by adding many PBR layers, your material will turn solid pink. If this happens, there are two potential options going forward: Option one
is to hide one or more lower layers while you work on new layers. Option two is to take advantage of the __Merge Visible__ tool (discussed
more in the following sections), which will merge all of the currently visible active layers into a single layer.