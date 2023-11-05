# Model

## 
```c#
Derives from Resource
```

## Summary

A model.
## Properties

```c#
static ModelBuilder Builder { get; } 
```
Returns a staticSandbox.ModelBuilderinstance, allowing for runtime model creation.
```c#
int AnimationCount { get; } 
```
Number of animations this model has.
```c#
AnimationGraph AnimGraph { get; } 
```
Get the animgraph this model uses.
```c#
int AttachmentCount { get; } 
```
Returns amount of attachment points this model has.
```c#
IEnumerable<BodyPart> BodyParts { get; } 
```
No Summary
```c#
int BoneCount { get; } 
```
Number of bones this model has.
```c#
BoneCollection Bones { get; } 
```
Access to bones of this model.
```c#
BBox Bounds { get; } 
```
Total bounds of all the meshes.
```c#
bool IsError { get; } 
```
Whether this model is an error model or invalid or not.
```c#
bool IsProcedural { get; } 
```
Whether this model is procedural, i.e. it was created at runtime viaModelBuilder.Create.
```c#
int MaterialGroupCount { get; } 
```
Number of material groups this model has.
```c#
IEnumerable<Material> Materials { get; } 
```
Retrieves an enumerable collection of all Materials on the meshes.
```c#
int MeshCount { get; } 
```
Total number of meshes this model is made out of.
```c#
int MorphCount { get; } 
```
Number of morph controllers this model has.
```c#
string Name { get; } 
```
Name of the model, usually being its file path.
```c#
PhysicsGroupDescription Physics { get; } 
```
No Summary
```c#
BBox PhysicsBounds { get; } 
```
Total bounds of all the physics shapes.
```c#
BBox RenderBounds { get; } 
```
Render view bounds.
```c#
MeshTraceRequest Trace { get; } 
```
Trace against the triangles in this mesh
## Methods

```c#
static Model Load( string filename) 
```
Load a model by file path.
```c#
string GetAnimationName( int animationIndex) 
```
Returns name of an animation at given animation index.
```c#
Transform? GetAttachment( string name) 
```
Retrieves attachment transform based on given attachment name.
```c#
Transform? GetAttachment( int index) 
```
Retrieves attachment transform based on given attachment index.
```c#
string GetAttachmentName( int index) 
```
Returns name of an attachment at given index.
```c#
string GetBoneName( int boneIndex) 
```
Returns name of a bone at given bone index.
```c#
int GetBoneParent( int boneIndex) 
```
Returns the id of given bone's parent bone.
```c#
Transform GetBoneTransform( int boneIndex) 
```
Returns transform of given bone at bind position.
```c#
Transform GetBoneTransform( string bone) 
```
Returns transform of given bone at bind position.
```c#
Dictionary<string, string[]> GetBreakCommands( ) 
```
Internal function used to get a list of break commands the model has.
```c#
T GetData<T,>( ) 
```
Extracts data from model based on the given type'sModelDoc.GameDataAttribute.
```c#
uint[] GetIndices( ) 
```
Experimental! Try to get all indices from model (meshes need to be compiled with CPU access!)
```c#
int GetMaterialGroupIndex( string groupIndex) 
```
Retrieves the index of a material group given its name.
```c#
string GetMaterialGroupName( int groupIndex) 
```
Returns name of a material group at given group index.
```c#
IEnumerable<Material> GetMaterials( int groupIndex) 
```
Retrieves an enumerable collection of Materials belonging to a specified group.
```c#
IEnumerable<Material> GetMaterials( string groupName) 
```
Retrieves an enumerable collection of Materials belonging to a specified group.
```c#
string GetMorphName( int morph) 
```
Returns name of a morph controller at given index.
```c#
float GetPhonemeMorph( int phoneme, int morph) 
```
Get morph weight for phoneme, this is only really needed for tools.
```c#
Vertex[] GetVertices( ) 
```
Experimental! Try to get all vertices from model (meshes need to be compiled with CPU access!)
```c#
bool HasData<T,>( ) 
```
Tests if this model has generic data based on given type'sModelDoc.GameDataAttribute.
This will be faster than testing this via GetData<>()
```c#
bool TryGetData<T,>( out T data) 
```
Tries to extract data from model based on the given type'sModelDoc.GameDataAttribute.
```c#
bool TryGetData( Type t, out object data) 
```
Tries to extract data from model based on the given type'sModelDoc.GameDataAttribute.
```c#
override string ToString( ) 
```
OverridesObject.ToString
## Extensions

```c#
List<T> GetAllData<T,>( ) 
```
Returns all game data nodes that derive from given class/interface, and are present on the model. Does NOT support data nodes that allow multiple entries.
## Nested Types

