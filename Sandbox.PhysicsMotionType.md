# PhysicsMotionType

## Derives from Enum

## Summary

RepresentsPhysics body'smotion type.
## Fields

```c#
static PhysicsMotionType Dynamic = 1
```
Physically simulated body.
```c#
static PhysicsMotionType Invalid = 0
```
Invalid type.
```c#
static PhysicsMotionType Keyframed = 3
```
No physics simulation, but can be moved via setting position/rotation.
```c#
static PhysicsMotionType Static = 2
```
Cannot move at all.
## Referencing Members

```c#
PhysicsGroup = ModelEntity.SetupPhysicsFromAABB( PhysicsMotionType, Vector3, Vector3 ) 
```
```c#
PhysicsGroup = ModelEntity.SetupPhysicsFromCapsule( PhysicsMotionType, Capsule ) 
```
```c#
PhysicsGroup = ModelEntity.SetupPhysicsFromCylinder( PhysicsMotionType, Capsule ) 
```
```c#
PhysicsGroup = PhysicsWorld.SetupPhysicsFromModel( Model, PhysicsMotionType ) 
```
```c#
PhysicsGroup = PhysicsWorld.SetupPhysicsFromModel( Model, Transform, PhysicsMotionType ) 
```
```c#
PhysicsGroup = ModelEntity.SetupPhysicsFromModel( PhysicsMotionType, bool ) 
```
```c#
PhysicsGroup = ModelEntity.SetupPhysicsFromOBB( PhysicsMotionType, Vector3, Vector3 ) 
```
```c#
PhysicsGroup = ModelEntity.SetupPhysicsFromOrientedCapsule( PhysicsMotionType, Capsule ) 
```
```c#
PhysicsGroup = ModelEntity.SetupPhysicsFromSphere( PhysicsMotionType, Vector3, float ) 
```
