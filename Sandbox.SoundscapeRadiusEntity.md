# SoundscapeRadiusEntity

## ```c#
Implements ISoundscapeEntity
```

## Summary

Declares a sphere in which the specified soundscape will be active. If the ear is within two radiuses, we'll use the
closest. The entity needs to be within the PVS for it to be active.
## Constructors

```c#
SoundscapeRadiusEntity( ) 
```
No Summary
## Properties

```c#
virtual string Soundscape { get; set; } 
```
ImplementsISoundscapeEntity.SoundscapeThe soundscape resource to play.
```c#
bool Enabled { get; set; } 
```
Whether the soundscape is active or not.
```c#
float Radius { get; set; } 
```
Radius of this soundscape.
## Methods

```c#
virtual void DrawDebugOverlays( ) 
```
ImplementsISoundscapeEntity.DrawDebugOverlaysCalled when debug overlay mode selected (in the editor) is "Soundscapes"
```c#
virtual bool TestPosition( Vector3 position) 
```
ImplementsISoundscapeEntity.TestPositionCalled by the soundscape system to test if a client is within soundscape bounds.
```c#
protected void Disable( ) 
```
Become disabled
```c#
protected void Enable( ) 
```
Become enabled
```c#
protected void Toggle( ) 
```
Toggle between enabled and disabled
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
