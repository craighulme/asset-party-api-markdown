# WaterExtensions

## Is static
Derives from object

## Summary

Adds functions to Entity
## Methods

```c#
static void ClearWaterLevel( IEntity self) 
```
Clear any current water level. Pretend we're not in water anymore.
Usually called on Respawn.
```c#
static float GetWaterLevel( IEntity self) 
```
Get the water level for this entity
