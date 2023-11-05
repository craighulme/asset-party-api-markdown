# AnimatedEntity

## Derives from ModelEntity

## Summary

A model entity that can also play animations and use animation graphs.
## Constructors

```c#
AnimatedEntity( ) 
```
No Summary
```c#
AnimatedEntity( string modelName) 
```
No Summary
```c#
AnimatedEntity( string modelName, IEntity parent) 
```
No Summary
## Properties

```c#
bool AnimateOnServer { get; set; } 
```
Whether this entity should animate on the server viaAnimatedEntity.CurrentSequence.
```c#
AnimationGraph AnimGraph { get; set; } 
```
Override the anim graph this entity uses
```c#
AnimationSequence CurrentSequence { get; } 
```
Allows playback of sequences directly, rather than using an animation graph.
RequiresAnimatedEntity.UseAnimGraphdisabled if the entity has one. Also seeAnimatedEntity.AnimateOnServer.
```c#
AnimGraphDirectPlayback DirectPlayback { get; } 
```
Access this entity's direct playback. Direct playback is used to control the direct playback node in an animgraph
to play sequences directly in code
```c#
float PlaybackRate { get; set; } 
```
Playback rate of the animations on this entity
```c#
Vector3 RootMotion { get; } 
```
Experimental root motion velocity for anim graphs that use root motion
```c#
float RootMotionAngle { get; } 
```
Experimental root motion angle velocity for anim graphs that use root motion
```c#
bool UseAnimGraph { get; set; } 
```
Allows the entity to not use the anim graph so it can play sequences directly
## Methods

```c#
protected virtual void OnAnimFootstep( bool leftFoot, Vector3 position) 
```
Called when an animation-driven footstep sound needs to be played.
```c#
protected virtual void OnAnimGraphCreated( ) 
```
An anim graph has been created for this entity. You will want to set up initial AnimGraph parameters here.
```c#
protected virtual void OnAnimGraphTag( string tag, AnimGraphTagEvent fireMode) 
```
Called when the anim graph of this entity has a tag change.
This will be called only for "Status" type tags.
```c#
protected virtual void OnAnimSound( string sound, string attachment) 
```
Called when an animation-driven sound needs to be played.
```c#
protected virtual void OnNewSequence( ) 
```
Called when a new animation sequence is set
```c#
protected virtual void OnSequenceFinished( bool looped) 
```
Called when an animation sequence has finished or looped
```c#
void CopyAnimParameters( AnimatedEntity from) 
```
Copy anim parameters from given entity.
```c#
bool GetAnimParameterBool( string name) 
```
Retrieve parameter value of currently active Animation Graph.
```c#
float GetAnimParameterFloat( string name) 
```
Retrieve parameter value of currently active Animation Graph.
```c#
int GetAnimParameterInt( string name) 
```
Retrieve parameter value of currently active Animation Graph.
```c#
Rotation GetAnimParameterRotation( string name) 
```
Retrieve parameter value of currently active Animation Graph.
```c#
Vector3 GetAnimParameterVector( string name) 
```
Retrieve parameter value of currently active Animation Graph.
```c#
float GetSequenceDuration( string sequenceName) 
```
Get the duration of a sequence by name
```c#
bool HasAnimGraph( ) 
```
Whether this entity's model has an anim graph or not
```c#
bool IsValidSequence( string sequenceName) 
```
Check whether a sequence is valid by name
```c#
void ResetAnimParameters( ) 
```
Reset all animgraph parameters to their default values
```c#
void SetAnimGraph( string name) 
```
Override the anim graph this entity uses
```c#
void SetAnimLookAt( string name, Vector3 eyePositionInWorld, Vector3 lookatPositionInWorld) 
```
Converts value to vector local to this entity's eyepos and passes it to SetAnimVector
```c#
void SetAnimParameter( string name, bool value) 
```
Sets the animation graph parameter.
```c#
void SetAnimParameter( string name, float value) 
```
Sets the animation graph parameter.
```c#
void SetAnimParameter( string name, Vector3 value) 
```
Sets the animation graph parameter.
```c#
void SetAnimParameter( string name, Rotation value) 
```
Sets the animation graph parameter.
```c#
void SetAnimParameter( string name, int value) 
```
Sets the animation graph parameter.
```c#
void SetAnimParameter( string name, Transform value) 
```
Sets the animation graph parameter.
## Extensions

```c#
void ProceduralHitReaction( DamageInfo info, float damageScale = 1) 
```
Sets the procedural hit creation parameters for the animgraph node, which makes the
model twitch according to where it got hit.The parameters set arebool hit
int hit_bone
vector hit_offset
vector hit_direction
vector hit_strength
## Nested Types

## Inheriting Types

