# CapsuleAttribute

## 
```c#
Derives from BaseTransformAttribute
```

## Summary

Draws a capsule, which can be manipulated via gizmos. You can have multiple of these.
## Constructors

```c#
CapsuleAttribute( string point1Key, string point2key, string radiusKey) 
```
This variation has 1 radius for both points.
```c#
CapsuleAttribute( string point1Key, string point2key, string radius1Key, string radius2Key) 
```
This variation has independent radius for each point.
## Methods

```c#
protected override void AddKeys( Dictionary<string, object> dict) 
```
OverridesBaseModelDocAttribute.AddKeysAdd generic key-values to the helper.
## Inheriting Types

