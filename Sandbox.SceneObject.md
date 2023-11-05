# SceneObject

## Derives from object
Implements IHandle

## Summary

A model scene object that can be rendered within aSandbox.SceneWorld.
## Constructors

```c#
SceneObject( SceneWorld sceneWorld, Model model) 
```
No Summary
```c#
SceneObject( SceneWorld sceneWorld, Model model, Transform transform) 
```
No Summary
```c#
SceneObject( SceneWorld sceneWorld, string modelName, Transform transform) 
```
No Summary
```c#
SceneObject( SceneWorld sceneWorld, string modelName) 
```
No Summary
## Properties

```c#
Angles Angles { get; set; } 
```
No Summary
```c#
RenderAttributes Attributes { get; } 
```
No Summary
```c#
bool Batchable { get; set; } 
```
This object is not batchable by material for some reason ( example: has dynamic attributes that affect rendering )
```c#
BBox Bounds { get; set; } 
```
Set or get the axis aligned bounding box for this object.
```c#
Plane ClipPlane { get; set; } 
```
Clipping plane for this scene object. RequiresSceneObject.ClipPlaneEnabledto betrue.
```c#
bool ClipPlaneEnabled { get; set; } 
```
Whether or not to use the clipping plane defined inSceneObject.ClipPlane.
```c#
Color ColorTint { get; set; } 
```
Color tint of this scene object.
```c#
SceneObjectFlagAccessor Flags { get; } 
```
Access to various advanced scene object flags.
```c#
BBox LocalBounds { get; set; } 
```
The world bounds translated to the local position. Note that this
does NOT do any scaling or rotation.
```c#
ulong MeshGroupMask { get; set; } 
```
State of all bodygroups of this object's model. You might be looking forSceneModel.SetBodyGroup.
```c#
Model Model { get; set; } 
```
The model this scene object will render.
```c#
SceneObject Parent { get; } 
```
Movement parent of this scene object, if any.
```c#
Vector3 Position { get; set; } 
```
Position of this scene object, relative to itsSceneObject.Parent, orSandbox.SceneWorldif parent is not set.
```c#
bool RenderingEnabled { get; set; } 
```
Whether this scene object should render or not.
```c#
SceneRenderLayer RenderLayer { get; set; } 
```
For a layer to draw this object, the target layer must match (or be unset)
and the flags must match
```c#
Rotation Rotation { get; set; } 
```
Rotation of this scene object, relative to itsSceneObject.Parent, orSandbox.SceneWorldif parent is not set.
```c#
ITagSet Tags { get; } 
```
List of tags for this scene object.
```c#
Transform Transform { get; set; } 
```
Transform of this scene object, relative to itsSceneObject.Parent, orSandbox.SceneWorldif parent is not set.
```c#
SceneWorld World { get; } 
```
The scene world this object belongs to.
## Methods

```c#
void AddChild( string name, SceneObject child) 
```
Add a named child scene object to this one. The child scene object will have its parent set.
```c#
void ClearMaterialOverride( ) 
```
Clear all material replacements.
```c#
void Delete( ) 
```
Delete this scene object. You shouldn't access it anymore.
```c#
void RemoveChild( SceneObject child) 
```
Unlink given scene object as a child from this one. The child scene object will have its parent set to null. It will not be deleted.
```c#
void SetMaterialGroup( string name) 
```
Set material group to replace materials of the model as set up in ModelDoc.
```c#
void SetMaterialOverride( Material material) 
```
Override all materials on this object'sSceneObject.Model.
```c#
void SetMaterialOverride( Material material, string attributeName, int attributeValue = 1) 
```
Replaces all materials of the model that have the givenUser Material Attributeset to"1", with given material.The system checks both the models' default material group materials and the materials of the active material group.
## Nested Types

## Inheriting Types

