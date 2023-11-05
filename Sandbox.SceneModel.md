# SceneModel

## 
```c#
Derives from SceneObject
```

## Summary

A model scene object that supports animations and can be rendered within aSandbox.SceneWorld.
## Constructors

```c#
SceneModel( SceneWorld sceneWorld, string model, Transform transform) 
```
No Summary
```c#
SceneModel( SceneWorld sceneWorld, Model model, Transform transform) 
```
No Summary
## Properties

```c#
AnimationGraph AnimationGraph { get; set; } 
```
No Summary
```c#
AnimationSequence CurrentSequence { get; } 
```
Allows playback of sequences directly, rather than using an animation graph.
RequiresSceneModel.UseAnimGraphdisabled if the scene model has one.
```c#
AnimGraphDirectPlayback DirectPlayback { get; } 
```
Access this sceneobject's direct playback. Direct playback is used to control the direct playback node in an animgraph
to play sequences directly in code
```c#
MorphCollection Morphs { get; } 
```
Access this sceneobject's morph collection. Morphs are generally used in the model to control
the face, for things like emotions and lip sync.
```c#
Action<FootstepEvent> OnFootstepEvent { get; set; } 
```
Called when a footstep event happens
```c#
Action<GenericEvent> OnGenericEvent { get; set; } 
```
Called when a generic event happens
```c#
Action<SoundEvent> OnSoundEvent { get; set; } 
```
Called when a sound event happens
```c#
bool UseAnimGraph { get; set; } 
```
Allows the scene model to not use the anim graph so it can play sequences directly
## Methods

```c#
void ClearBoneOverrides( ) 
```
No Summary
```c#
Transform? GetAttachment( string name, bool worldspace = true) 
```
Get attachment transform by name.
```c#
Transform GetBoneWorldTransform( int boneIndex) 
```
Returns the world space transform of a bone by its index.
```c#
Transform GetBoneWorldTransform( string boneName) 
```
Returns the world space transform of a bone by its name.
```c#
bool GetBool( string name) 
```
Get an animated parameter
```c#
float GetFloat( string name) 
```
Get an animated parameter
```c#
int GetInt( string name) 
```
Get an animated parameter
```c#
Rotation GetRotation( string name) 
```
Get an animated parameter
```c#
Vector3 GetVector3( string name) 
```
Get an animated parameter
```c#
void MergeBones( SceneModel parent) 
```
Update our bones to match the target's bones. This is a manual bone merge.
```c#
void ResetAnimParameters( ) 
```
Reset all animgraph parameters to their default values.
```c#
void RunPendingEvents( ) 
```
No Summary
```c#
void SetAnimGraph( string name) 
```
No Summary
```c#
void SetAnimParameter( string name, bool value) 
```
Sets a boolean animation graph parameter by name.
```c#
void SetAnimParameter( string name, float value) 
```
Sets a float animation graph parameter by name.
```c#
void SetAnimParameter( string name, Vector3 value) 
```
Sets a vector animation graph parameter by name.
```c#
void SetAnimParameter( string name, int value) 
```
Sets a integer animation graph parameter by name.
```c#
void SetAnimParameter( string name, Rotation value) 
```
Sets a rotation animation graph parameter by name.
```c#
void SetBodyGroup( string name, int value) 
```
Set which body group to use.
```c#
void SetBoneOverride( int boneIndex, in Transform transform, float lerp = 1) 
```
No Summary
```c#
void SetBoneWorldTransform( int boneIndex, Transform transform) 
```
Sets the world space bone transform of a bone by its index.
```c#
void SetMaterialGroup( string name) 
```
ImplementsSceneObject.SetMaterialGroupSet material group to replace materials of the model as set up in ModelDoc.
```c#
void Update( float delta) 
```
Update this animation. Delta is the time you want to advance, usually RealTime.Delta
```c#
void UpdateToBindPose( ) 
```
Update all of the bones to the bind pose
## Nested Types

