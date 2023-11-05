# Bone

## 
```c#
Derives from object
```

## Summary

A bone in aSandbox.BoneCollection.
## Constructors

```c#
protected Bone( ) 
```
No Summary
## Properties

```c#
virtual bool HasChildren { get; } 
```
Whether this bone has any child bones.
```c#
virtual int Index { get; } 
```
Numerical index of this bone.
```c#
virtual Transform LocalTransform { get; } 
```
Transform on this bone, relative to the root bone.
```c#
virtual string Name { get; } 
```
Name of this bone.
```c#
virtual Bone Parent { get; } 
```
The parent bone.
```c#
IReadOnlyList<Bone> Children { get; } 
```
List of all bones that descend from this bone.
## Methods

```c#
bool IsNamed( string name) 
```
Whether this bone has given name or not.
