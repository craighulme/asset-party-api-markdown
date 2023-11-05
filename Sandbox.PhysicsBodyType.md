# PhysicsBodyType

## 
```c#
Derives from Enum
```

## Summary

Physically simulated body.
## Fields

```c#
static PhysicsBodyType Dynamic = 2
```
Physically simulated body.
```c#
static PhysicsBodyType Keyframed = 1
```
No physics simulation, but can be moved via setting position/rotation.
```c#
static PhysicsBodyType Static = 0
```
Cannot move at all.
## Referencing Members

```c#
PhysicsBodyType = PhysicsBody.BodyType { get; set; } 
```
