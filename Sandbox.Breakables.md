# Breakables

## 
```c#
Derives from object
```

## Summary

Handle breaking a prop into bits
## Properties

```c#
static int MaxGibs { get; set; } 
```
How many gibs spawned by this class are allowed to exist at any given time.
## Methods

```c#
static void Break( Entity ent, Result result = null) 
```
Create gibs based on entity's model and other characteristics.
```c#
static void Break( Model model, Vector3 pos, Rotation rot, float scale, Color color, Result result = null, PhysicsBody sourcePhysics = null) 
```
Create gibs of given model, at given position, rotation and scale, with given color.
## Nested Types

