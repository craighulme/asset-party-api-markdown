# Result

## 
```c#
Derives from object
```

## Summary

Allows to retrieve resulting gib entities, and pass some extra information when generating gibs.
## Constructors

```c#
Result( ) 
```
No Summary
## Fields

```c#
BreakableParams Params
```
Various break piece related parameters
```c#
List<ModelEntity> Props
```
List of gibs generated. Amount of gibs may not match model's break piece count depending on value ofBreakables.MaxGibs.
```c#
Entity Source
```
The entity that is breaking.
## Methods

```c#
void AddProp( ModelEntity prop) 
```
Add an entity to thegenerated gibs list.
```c#
void CopyParamsFrom( DamageInfo dmgInfo) 
```
Copy useful parameters from a damage info object for gib randomization andbreak commands.
## Nested Types

