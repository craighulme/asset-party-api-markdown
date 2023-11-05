# Clothing

## ```c#
Derives from GameResource
```

## Summary

A piece of player model customization.
## Constructors

```c#
Clothing( ) 
```
No Summary
## Properties

```c#
ClothingCategory Category { get; set; } 
```
What kind of clothing this is?
```c#
string EyesMaterial { get; set; } 
```
Replace the eyes with this material
```c#
BodyGroups HideBody { get; set; } 
```
Which body parts of the player model should not show when this clothing is equipped.
```c#
IconSetup Icon { get; set; } 
```
Icon for this clothing piece.
```c#
string MaterialGroup { get; set; } 
```
Which material group of the model to use.
```c#
string Model { get; set; } 
```
The model to bonemerge to the player when this clothing is equipped.
```c#
Clothing Parent { get; set; } 
```
The clothing to parent this too.  It will be displayed as a variation of its parent
```c#
string SkinMaterial { get; set; } 
```
Replace the skin with this material
```c#
Slots SlotsOver { get; set; } 
```
Which slots this clothing takes on "outer" layer.
```c#
Slots SlotsUnder { get; set; } 
```
Which slots this clothing takes on "inner" layer.
```c#
string SubCategory { get; set; } 
```
This should be a single word to describe the subcategory, and should match any other items you want to categorize in the same bunch. The work will be tokenized so it can become localized.
```c#
string Subtitle { get; set; } 
```
A subtitle for this clothing piece.
```c#
string Title { get; set; } 
```
Name of the clothing to show in UI.
## Methods

```c#
static List<SceneModel> DressSceneObject( SceneModel citizen, IEnumerable<Clothing> Clothing) 
```
Dress this sceneobject with the passed clothes. Return the created clothing.
```c#
bool CanBeWornWith( Clothing target) 
```
Return true if this item of clothing can be worn with the target item, at the same time.
## Nested Types

