# User Interface
The ToAutomate UI is located in the Properties(Press N) Panel of the 3D-View.

## Side Panel
<img src= "/assets/images/ToAutomate_Main.png", width="600"> <br>
Located in the Properties Panel of 3D View, Tap `To Automate` to get started and you'll see following tool menus.

## 3D Object Tools
<img src= "/assets/images/3D_Tools.png", width="300"> <br>

1. **Rename**: Select Two Object and press `Rename`, It Renames the active Object and add '_LP' suffix to it and '_HP' suffix to the other selected object
    1. Rename Operator requires two selected object to make a Low-High Object named Pair
    1. On Press of Rename, the active Object (named "Cube") get renamed to Cube + "_LP" (`Low Suffix`) and second selected object get renamed Cube + "_HP" (High Suffix)
    2. Resulting name of active_object becomes from "Cube" to "Cube_LP"<br>
        and for `second` selected object "Cube_HP", <br>High_name = Low_object_name + high_suffix

2. **Object Organize Method**
    1. Method to Organize: 
        1. `OP1`: Separate Low-High:  When pressed Rename, Moves the Low and High suffix objects to the individual `Low_Col` and `High_Col` Collections respectively.<br> Toggle the `Check` in front of LP Col and HP Col to disable moving to collection.
        2. `OP2`: Object Collection: When pressed Rename, Moves both the Low and High suffixed objects to a new `Object's name` Collection. <br> **Example:** Resulting `"Cube_LP"` and `"Cube_HP"` Objects will both be in Collection `"Cube"`.
3. **Selection Menu**:
    1. `OP1`: To Check if an object's counterpart (Low or high) exists.
    2. `OP2`: To Check if any object doesn't have it's Counterpart (Low or high) and select them.
    3. `Note`: Works with respect to defined/named LP Col and HP Col in Organize Method 

4. **Collection Organizer**: Converts the Blender's Collection Heirarchy to Empty object-parent collection for the collection tree, Helpful when want to preserve heirarchy for .fbx or other 3D softwares.
    1. `Source Col`: Select a Source Collection to Convert to Empty-object Parent heirarchy.
    2. `Parent`: Toggle Parent if we want an external Empty-Object that will go on top of the Final src Collection object.
        3. `Name`: Give a name for the External Parent Object, If doesn't exist, will create it
    3. `Organize`: Press Organize and convert your Collection Heirarchy into empty-parent heirarchy

## Mesh Menu
<img src= "/assets/images/Mesh_Operators.png", width="300"> <br>

1. **Modifiers**:
    1. Overview: Applies the following Modifiers to all selected objects.
    1. `Create New`: If the object already have selected modifier, It'll create an additional new modifier. Helpful when need multiple Mirror Modifiers.
    2. `TRIANGULATE`: Apply to all objects, keeps mesh clean to edit and prepared for export and baking. <br>
    Adds a triangulate modifier, with `keep normals` toggled `On` (Helpful in keeping normals consistent).
    3. `MIRROR`: Adds a Mirror Modifier to selected object, with some additional properties as a pop up menu.
        1. Opens an Additional Dialogue menu to select the Mirror Origin (A symmetry Object in world center). Or to Select axis for the mirror.
        2. Applies to all selected objects
    4. `Dynamic Array`: It's not normal array, it needs two objects specifically. What it does basically is: 
        1. `Requirements`: The active object and a second selected object
        2. Dynamic Array calculates the 3D Distance between both objects and adds an array to active object that makes it's Array distance to the calculated distance above.
        3. `Weighted Normal`: Adds Weighted Normal to all the selected objects.
        4. `SHIFT UV`: Helpful for Mirrors and Arrays, When in game object baking, having mirror for each object, can result in Overlap UVs, so enable SHIFT_UV, and select U or V or both to shift the Mirrored-part's UV out of 1:1 to avoid overlap in main baking region.
2. **Materials**
    1. `Material`: Select a Material from Scene
    2. `Delete Old Material`: Toggle ON to remove old materials of an object, when adding material from below.
    3. `Add Material`: Adds selected Material in `Material` to all selected objects.
        1. If no `Material` was selected, a pop-up will come up that asks for a name for the New Material to add to the objects.
    4. `Del Materials`: Deletes all Materials of all selected Objects. Everything
    4. `Clean UP`: Removes Unused Materials from selected Objects.
 


## UV Menu
<img src= "/assets/images/UV_Operators.png", width="300"> <br>

## Export Menu
<img src= "/assets/images/Export_System_Closed.png", width="300", style="vertical-align: top;">
<img src= "/assets/images/Export_System_Exp.png", width="300", style="vertical-align: top;>


