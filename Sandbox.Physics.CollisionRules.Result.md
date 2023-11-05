# Result

## 
```c#
Derives from Enum
```

## Summary

Result of a collision betweentwo objects.
## Fields

```c#
static Result Collide = 3
```
Collide.
```c#
static Result Ignore = 1
```
Do not collide.
```c#
static Result Trigger = 2
```
Do not collide, but trigger touch callbacks.
```c#
static Result Unset = 0
```
Fallback to default behavior.
## Referencing Members

```c#
Dictionary<string, Result> = CollisionRules.Defaults { get; set; } 
```
```c#
Result = CollisionMatrixWidget.FindPair( string, string ) 
```
```c#
Pair.Pair( string, string, Result ) 
```
```c#
Result = Pair.Result { get; set; } 
```
```c#
void CollisionMatrixWidget.SetPair( string, string, Result ) 
```
