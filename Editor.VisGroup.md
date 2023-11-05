# VisGroup

## ```c#
Derives from Enum
```

## Summary

Used to tell Hammer which automatic Visibility Groups an entity should belong to. SeeVisGroupAttribute.
## Fields

```c#
static VisGroup Dynamic = 7
```
Entities that do not move via physics but are still intractable with or otherwise non static.
```c#
static VisGroup Lighting = 0
```
Entities that are primarily lights and that sort of thing.
```c#
static VisGroup Logic = 2
```
Pure logic entities, typically not shown in-game.
```c#
static VisGroup Navigation = 4
```
Entities that are related to nav meshes.
```c#
static VisGroup Particles = 5
```
The main reason these exist is to create particle systems.
```c#
static VisGroup Physics = 6
```
Physics enabled entities.
```c#
static VisGroup Sound = 1
```
The purpose of these entities is to emit light and not much else.
```c#
static VisGroup Trigger = 3
```
Any sort of trigger volume, these usually don't show up in-game.
## Referencing Members

```c#
VisGroup = VisGroupAttribute.Group { get; set; } 
```
```c#
VisGroupAttribute.VisGroupAttribute( VisGroup ) 
```
