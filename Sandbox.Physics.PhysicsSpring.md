# PhysicsSpring

## Derives from ValueType

## Summary

Spring related settings for joints such asPhysics.FixedJoint.
## Constructors

```c#
PhysicsSpring( float frequency = 0, float damping = 0, float maximum = 0) 
```
No Summary
## Fields

```c#
float Damping
```
The damping ratio of the spring, usually between 0 and 1
```c#
float Frequency
```
The stiffness of the spring
```c#
float Maximum
```
For weld joints only, maximum force. Not for breaking.
## Operators

```c#
implicit Vector3 =( PhysicsSpring s) 
```
No Summary
```c#
implicit PhysicsSpring =( Vector3 s) 
```
No Summary
## Referencing Members

```c#
PhysicsSpring = FixedJoint.SpringAngular { get; set; } 
```
```c#
PhysicsSpring = FixedJoint.SpringLinear { get; set; } 
```
```c#
PhysicsSpring = SpringJoint.SpringLinear { get; set; } 
```
```c#
PhysicsSpring = PhysicsSpringProperty.Value { get; set; } 
```
