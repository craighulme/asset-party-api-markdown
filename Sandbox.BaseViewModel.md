# BaseViewModel

## Derives from AnimatedEntity

## Summary

A common base we can use for weapons so we don't have to implement the logic over and over
again.
## Constructors

```c#
BaseViewModel( ) 
```
No Summary
## Fields

```c#
static List<BaseViewModel> AllViewModels
```
All active view models.
## Methods

```c#
virtual void PlaceViewmodel( ) 
```
Position your view model here.
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
```c#
override void OnNewModel( Model model) 
```
OverridesModelEntity.OnNewModelCalled when the model of this entity has changed.
```c#
override Sound PlaySound( string soundName, string attachment) 
```
OverridesEntity.PlaySoundPlay a sound from this entity at given attachment point, updating sounds' position as the entity and its attachments move.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
