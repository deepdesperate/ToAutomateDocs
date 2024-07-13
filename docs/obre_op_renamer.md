# Renamer Operator

### Rename Low & High Poly Objects Appropriately

![Renamer UI](assets/images/Ovw_Rename.jpg)

#### Properties:
1. `LP_Suffix`: Set suffix that will be added to the Low Poly Object
2. `HP_Suffix`: Set suffix that will be added to the High Poly Object
3. `LP Collection`: Set name for the Low poly collection to hold LP Objects
4. `HP Collection`: Set name for the Low poly collection to hold HP Objects
5. `Operator`: Rename Button to run the algorithm and rename object

#### Example:
1. Select two objects `active_object` and `second_object`, when the algorithm runs, it will rename the `active_object` and add LP suffix to it. And adds the HP suffix to the non-active object.
2. If you have toggled the `Move to Collection` property to `ON`. It will move the respective object with the respective name to the respective Collection.
3. For example, if you had LP prefix as `_LP`, and HP prefix as `_HP`, and name will become: `my_obj_name__LP` and `my_obj_name_HP` for HP, and they will be moved to the `LP` and `HP` Collection respectively.

### Selection Menu
**Requirements**: Works with the collections and Suffix of the Rename operators. Like LP & HP suffix and LP & HP Collection Names.

**Options**

1. `Select non-matching object`: Search for objects that doesn't have matching counterparts in the opposite collection. Like finding if no HP object of `abc_LP`   
2. `Select significant other`: Selects the HP object of selected LP objects or vice versa. Helpful when needed to select counter object of selected objects.

## How To Use