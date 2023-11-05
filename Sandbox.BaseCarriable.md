# BaseCarriable

## 
```c#
Derives from AnimatedEntity
```

## Summary

Utility - return the entity we should be spawning particles from etc
## Constructors

```c#
BaseCarriable( ) 
```
No Summary
## Properties

```c#
virtual ModelEntity EffectEntity { get; } 
```
Utility - return the entity we should be spawning particles from etc
```c#
virtual string ViewModelPath { get; } 
```
No Summary
```c#
BaseViewModel ViewModelEntity { get; protected set; } 
```
No Summary
## Methods

```c#
virtual void ActiveEnd( Entity ent, bool dropped) 
```
This entity has stopped being the active entity. This most
likely means a player was holding it but has switched away
or dropped it (in which case dropped = true)
```c#
virtual void ActiveStart( Entity ent) 
```
This entity has become the active entity. This most likely
means a player was carrying it in their inventory and now
has it in their hands.
```c#
virtual bool CanCarry( Entity carrier) 
```
No Summary
```c#
virtual void CreateHudElements( ) 
```
No Summary
```c#
virtual void CreateViewModel( ) 
```
Create the viewmodel. You can override this in your base classes if you want
to create a certain viewmodel entity.
```c#
virtual void DestroyHudElements( ) 
```
No Summary
```c#
virtual void DestroyViewModel( ) 
```
We're done with the viewmodel - delete it
```c#
virtual void OnCarryDrop( Entity dropper) 
```
No Summary
```c#
virtual void OnCarryStart( Entity carrier) 
```
No Summary
```c#
virtual void SimulateAnimator( CitizenAnimationHelper anim) 
```
No Summary
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
## Inheriting Types

