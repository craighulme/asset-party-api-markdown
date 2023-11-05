# PropGib

## ```c#
Derives from Prop
```

## Summary

Used to track individual break pieces for the purposes of Model Break Commands.
ModelDoc guarantees that these names will be unique.
## Constructors

```c#
PropGib( ) 
```
No Summary
## Properties

```c#
string BreakpieceName { get; set; } 
```
Used to track individual break pieces for the purposes of Model Break Commands.
ModelDoc guarantees that these names will be unique.
## Methods

```c#
override void Spawn( ) 
```
OverridesProp.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
