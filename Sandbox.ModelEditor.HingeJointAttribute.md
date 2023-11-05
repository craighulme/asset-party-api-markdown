# HingeJointAttribute

## Derives from BaseTransformAttribute

## Summary

A helper that draws axis of rotation and angle limit of a hinge joint.
## Constructors

```c#
HingeJointAttribute( ) 
```
No Summary
## Properties

```c#
string EnableLimit { get; set; } 
```
Key name that dictates whether the hinge limit is enabled or not.
```c#
string MaxAngle { get; set; } 
```
Key name that stores the maximum angle value for the revolute joint.
```c#
string MinAngle { get; set; } 
```
Key name that stores the minimum angle value for the revolute joint.
## Methods

```c#
protected override void AddKeys( Dictionary<string, object> dict) 
```
OverridesBaseModelDocAttribute.AddKeysAdd generic key-values to the helper.
