# Animate

## Is static
Derives from object

## Summary

Add a float animation for this object
## Methods

```c#
static void Add( object owningObject, float secondsToTake, float from, float to, Action<float> value, string ease = "ease-in-out") 
```
Add a float animation for this object
```c#
static void CancelAll( object owningObject, bool jumpToEnd) 
```
Cancel all of this object's active animations
```c#
static void Frame( ) 
```
No Summary
```c#
static bool IsActive( object owningObject) 
```
Returns true if this object has any active animations
