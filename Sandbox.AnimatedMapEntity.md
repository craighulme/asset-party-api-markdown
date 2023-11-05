# AnimatedMapEntity

## ```c#
Derives from AnimatedEntity
```

## Summary

A static prop that can play animations. If a door is wanted, please use the door entity.
## Constructors

```c#
AnimatedMapEntity( ) 
```
No Summary
## Properties

```c#
bool Breakable { get; set; } 
```
If the model supports break pieces and has prop_data with health, this option can be used to allow the door to break like a normal prop would.
```c#
protected Output OnBreak { get; set; } 
```
Fired when the entity gets destroyed.
```c#
protected Output OnDamaged { get; set; } 
```
Fired when the entity gets damaged, even if it is unbreakable.
## Methods

```c#
void Break( ) 
```
Causes this prop to break, regardless if it is actually breakable or not. (i.e. ignores health and whether the model has gibs)
```c#
protected void DeleteInput( ) 
```
Deletes this prop.
```c#
void SetAnimation( string name) 
```
Play a specific animation (sequence) on the entity.
The parameter should be the name of the animation.
```c#
protected void SetBodyGroupInput( string group) 
```
Sets the body group of the props' model by name, as set in ModelDoc.
Format is "name,option"
```c#
protected void SetCollisions( bool enabled) 
```
Enables or disables collisions on this prop.
```c#
protected void SetMaterialGroupInput( string group) 
```
Sets the material group of the props' model by name, as set in ModelDoc.
```c#
protected void SetScale( float scale) 
```
Sets the scale of the prop, affecting physics and visual scale.
```c#
protected void SetVisible( bool enabled) 
```
Enables or disables collisions on this prop.
```c#
override void OnClientActive( IClient cl) 
```
OverridesEntity.OnClientActiveCalled when a player becomes active
```c#
override void OnKilled( ) 
```
OverridesEntity.OnKilledCalled (fromEntity.TakeDamageby default unless overridden) when there's no health left.
```c#
override void OnNewModel( Model model) 
```
OverridesModelEntity.OnNewModelCalled when the model of this entity has changed.
```c#
protected override void OnSequenceFinished( bool looped) 
```
OverridesAnimatedEntity.OnSequenceFinishedCalled when an animation sequence has finished or looped
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
```c#
override void TakeDamage( DamageInfo info) 
```
OverridesEntity.TakeDamageCalled when the entity receives a damage event. This is where you want to subtract health, etc.
## Inheriting Types

