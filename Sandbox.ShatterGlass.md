# ShatterGlass

## Derives from ModelEntity

## Summary

A procedurally shattering glass panel.
## Constructors

```c#
ShatterGlass( ) 
```
No Summary
## Properties

```c#
string BrokenMaterial { get; set; } 
```
Material to use for the glass when it is broken. If not set, the material will not change on break.
```c#
ShatterGlassConstraint Constraint { get; } 
```
Glass constraint.Glass with static edgeswill not be affected by gravity (glass pieces will) and will shatter piece by piece.Physics glassis affected by gravity and will shatter all at the same time.Physics but asleepis same as physics but will not move on spawn.
```c#
string DamagePositioningEntity { get; set; } 
```
If set, the glass will shatter at the position of this entity on spawn.
```c#
string DamagePositioningEntity02 { get; set; } 
```
If set, the glass will shatter at the position of this entity on spawn.
```c#
string DamagePositioningEntity03 { get; set; } 
```
If set, the glass will shatter at the position of this entity on spawn.
```c#
string DamagePositioningEntity04 { get; set; } 
```
If set, the glass will shatter at the position of this entity on spawn.
```c#
Vector3 FaceAxisForward { get; set; } 
```
No Summary
```c#
Vector3 FaceAxisRight { get; set; } 
```
No Summary
```c#
Vector4 FaceAxisU { get; set; } 
```
No Summary
```c#
Vector4 FaceAxisV { get; set; } 
```
No Summary
```c#
Vector3 FaceCenter { get; set; } 
```
No Summary
```c#
Vector2 FaceTexScale { get; set; } 
```
No Summary
```c#
Vector2 FaceTexSize { get; set; } 
```
No Summary
```c#
string FaceVertices { get; set; } 
```
No Summary
```c#
float HalfThickness { get; } 
```
No Summary
```c#
Transform InitialTransform { get; } 
```
Transform at spawn time used forShatterGlass.Reset.
```c#
bool IsBroken { get; set; } 
```
Whether this glass pane has shattered at least once.
```c#
string Material { get; set; } 
```
Material to use for the glass
```c#
int NumShards { get; } 
```
Number of shards that came from this shatter glass pane.
```c#
Output OnBreak { get; set; } 
```
Fired when the panel initially breaks.
```c#
Vector2 PanelSize { get; } 
```
Size of the unbroken glass pane.
```c#
IEnumerable<GlassShard> Shards { get; } 
```
All shards that came from this shatter glass pane.
```c#
float Thickness { get; } 
```
Thickness of the glass
## Methods

```c#
static void ResetGlassCommand( ) 
```
No Summary
```c#
void Break( ) 
```
Breaks the glass at its center.
```c#
GlassShard CreateNewShard( GlassShard parentShard) 
```
No Summary
```c#
void RemoveShard( GlassShard shard) 
```
No Summary
```c#
void Reset( ) 
```
Cleans up broken shards and creates a new primary shard
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
## Nested Types

