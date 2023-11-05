# CollisionEntityData

## ```c#
Derives from ValueType
```

## Summary

Data on one of the two entities involved in a collision, part ofSandbox.CollisionEventData.
## Fields

```c#
Entity Entity
```
Which entity we came in contact with.
```c#
PhysicsShape PhysicsShape
```
Our physics shape that caused the collision.
```c#
Vector3 PostAngularVelocity
```
Our angular impulse after the collision happened.AngularImpulse are exponential maps (an axis scaled by a "twist" angle in radians)
```c#
Vector3 PostVelocity
```
Ourvelocityafter the collision happened.
```c#
Vector3 PreAngularVelocity
```
Our angular impulse before the collision happened.AngularImpulse are exponential maps (an axis scaled by a "twist" angle in radians)
```c#
Vector3 PreVelocity
```
Ourvelocitybefore the collision happened.
```c#
Surface Surface
```
The surface the collision happened on.
## Referencing Members

```c#
CollisionEntityData = CollisionEventData.Other
```
```c#
CollisionEntityData = CollisionEventData.This
```
