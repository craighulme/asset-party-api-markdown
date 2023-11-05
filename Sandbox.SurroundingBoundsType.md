# SurroundingBoundsType

## 
```c#
Derives from Enum
```

## Summary

Dictates how surrounding bounds (Entity.WorldSpaceBounds) of an entity as calculated.
## Fields

```c#
static SurroundingBoundsType Hitboxes = 2
```
Expand the surrounding bounds to encompass all hitboxes of the model.
```c#
static SurroundingBoundsType ObjectBoundingBox = 0
```
To contain the object's OBB.
```c#
static SurroundingBoundsType Physics = 1
```
The most expensive option. Work it out using the physics objects.
If it's a ragdoll it'll contain each physics object.
## Referencing Members

```c#
SurroundingBoundsType = ModelEntity.SurroundingBoundsMode { get; set; } 
```
