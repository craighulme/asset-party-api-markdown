# BaseWeapon

## ```c#
Derives from BaseCarriable
```

## Summary

Does a trace from start to end, does bullet impact effects. Coded as an IEnumerable so you can return multiple
hits, like if you're going through layers or ricocheting or something.
## Constructors

```c#
BaseWeapon( ) 
```
No Summary
## Properties

```c#
virtual float PrimaryRate { get; } 
```
No Summary
```c#
virtual float SecondaryRate { get; } 
```
No Summary
```c#
TimeSince TimeSincePrimaryAttack { get; set; } 
```
No Summary
```c#
TimeSince TimeSinceSecondaryAttack { get; set; } 
```
No Summary
## Methods

```c#
virtual void AttackPrimary( ) 
```
No Summary
```c#
virtual void AttackSecondary( ) 
```
No Summary
```c#
virtual bool CanPrimaryAttack( ) 
```
No Summary
```c#
virtual bool CanReload( ) 
```
No Summary
```c#
virtual bool CanSecondaryAttack( ) 
```
No Summary
```c#
virtual void Reload( ) 
```
No Summary
```c#
virtual IEnumerable<TraceResult> TraceBullet( Vector3 start, Vector3 end, float radius = 2) 
```
Does a trace from start to end, does bullet impact effects. Coded as an IEnumerable so you can return multiple
hits, like if you're going through layers or ricocheting or something.
```c#
override Sound PlaySound( string soundName, string attachment) 
```
OverridesEntity.PlaySoundPlay a sound from this entity at given attachment point, updating sounds' position as the entity and its attachments move.
```c#
override void Simulate( IClient player) 
```
OverridesEntity.SimulateCalled when simulating as part of a player's tick. Like if it's a pawn.
```c#
override void Spawn( ) 
```
OverridesBaseCarriable.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
