# Object Renamer

Object Renamer

## Overview
Collection of blender tools to optimize different Game-artist workflows.

1. Object Renamer is a Blender addon aimed to optimize the **game-dev/artist** workflows in real production workflow.
2. It is an in-development addon which tackles various stages of production that could be optimized to simplify repetetive tasks and let artist focus on creative work.
3. Tools like **Renaming objects for LP/HP Baking stages, Pre-bake mesh Check, Collection Organizer, Modifier for group objects, UV-tools and lastly my fav: Export Tools**
4. This addon is always in an evolving stage to offer newer tools for workflows.
5. Developed by me, I work as a freelance Vehicle Artist, trying to adapt to my different clients, and I find different things to impprove with each encounter.

## Feature Overview

* `Object Rename` operator that can rename objects based on the active object, like active_object_LP, active_object_HP with option to move the suffix objects to their defined collections
* `Selection Menu` tool to find the **Low-Poly/High-Poly** counterparts of each other in scene or ur desired collection.
* `Collection Organization` tools to convert blender collection heirarchy into empty parents heirarchy, useful when u export from blender to unity when you want to preserve the collection heirarchy.
* `Move objects` tool to move group of objects to defined collection quickly with additional options.
* `Object Linker` tool to help object link to more than on one collection in **Blender.**
* `Modifiers Tools` Set of simple modifiers with options helpful to game-dev to add to multiple selected objects in scene.
    - Additional option for adding/modify depending on whether object already has the modifier.
* `Material Menu` To add material to multiple objects at once
* `Mesh tools` tools for small mesh operations:
    * Tool to make duplicates of the active objects but to the positions of the selected objects (other than active objects).
    * Tools to make linked-objects single user quickly.
* `UV Menu` Tools to check **UV-offset** in object modifiers
    * `UV Name` tools to create new UVs to selected objects, rename UVs, select specific UV to be active for view or render.
* `Export Tools` Tools for Creating different configuration of Exporting objects
    * `Collection Export` Select a Collection to include it and it's children to export, exclude any specific collection to remove from the final export.
    * `Export location` directory to export object into.
    * `Substance Opener` creates substance painter file with the exported file above and opens the Substance Painter project with it or creates new.


## Why Object Renamer Tools?
The tool is oriented towards production stages where efficiency is appreciated. I can't force any of my workflows or tools to anyone. But I am pretty sure, trying out these features for yourself can save a minute or two during each time you worked on a difficult workflow.

- Like finding which Low poly object doesn't have it's High Poly created or named wrongly in collection of 100s of those objects, or checking for multiple mesh of same LP/HP relationship.
- Exporting Specific Collections for **Normal-Baking**, and different final mesh for **Exporting**, Option to exclude any Collection from the Collection tree, just define a quick preset in Export Manager for the workflow and it will export the collection tree without you manually selecting each collection each time.
- **UV-Tools** UV Tools to help check whether every Baking objects has their Mirror/Array modifiers have offset, so they don't bake artifacts by mistake due to inverted mesh overlapping.
- At the end of the day, we want to work on our projects/task, with minimum bugs, export and baking mesh just to find out that one mesh wasn't named properly or somehow that one didn't have UV offset, that cycle can go repeatedly and in a game-dev environment can be frustrating.

## Getting Started
### Download and Installation
Install from our github or gumroad, gumroad is helpful just in case you wanna be notified of new releases. 

