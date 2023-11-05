# KeyframeEntity

## 
```c#
Derives from AnimatedEntity
```

## Summary

An entity that is moved programmatically. Like an elevator
or a linear smashing star wars garbage compactor
## Constructors

```c#
KeyframeEntity( ) 
```
No Summary
## Methods

```c#
virtual bool TryKeyframeTo( Transform pos) 
```
Used by KeyframeTo methods to try to move to a given transform
```c#
virtual bool TryLocalKeyframeTo( Vector3 pos, float delta) 
```
Used by KeyframeTo methods to try to move to a given local position
```c#
virtual bool TryLocalRotateTo( Rotation pos) 
```
Used by LocalRotateKeyframeTo to try to rotate to a given rotation
```c#
Task<bool> KeyframeTo( Transform target, float seconds, Function easing = null) 
```
Move to given transform in given amount of time
```c#
Task<bool> LocalKeyframeTo( Vector3 deltaTarget, float seconds, Function easing = null) 
```
Move to a given local position in given amount of time
```c#
Task<bool> LocalRotateKeyframeTo( Rotation localTarget, float seconds, Function easing = null) 
```
Rotate to a given local rotation in given amount of time
## Inheriting Types

