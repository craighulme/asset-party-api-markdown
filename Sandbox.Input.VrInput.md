# VrInput

## 
```c#
Derives from ValueType
```

## Summary

Position and rotation of the Head Mounted Display in local space coordinates.
## Properties

```c#
Transform Head { get; } 
```
Position and rotation of the Head Mounted Display in local space coordinates.
```c#
bool IsActive { get; } 
```
Whether VR is currently being used.
```c#
bool IsKnuckles { get; } 
```
Returns true if this is an index
```c#
bool IsRift { get; } 
```
Returns true if this is a rift or a touch
```c#
bool IsVive { get; } 
```
Returns true if this is a vive
```c#
VrHand LeftHand { get; } 
```
Information about the left hand input.
```c#
VrHand RightHand { get; } 
```
Information about the right hand input.
```c#
IReadOnlyList<TrackedObject> TrackedObjects { get; } 
```
No Summary
```c#
string Type { get; } 
```
Returns the headset type - like "vive", "touch", "rift". Returns empty string if unknown.
## Referencing Members

```c#
static VrInput = Input.VR { get; } 
```
