# DragEvent

## 
```c#
Derives from object
```

## Summary

Information about a widget drag and drop event.
## Constructors

```c#
DragEvent( ) 
```
No Summary
## Properties

```c#
DropAction Action { get; set; } 
```
Set this to what action will be (or was) performed.
```c#
DragData Data { get; } 
```
The drag data.
```c#
bool HasAlt { get; } 
```
WhetherAltkey was being held down at the time of the event.
```c#
bool HasCtrl { get; } 
```
WhetherControlkey was being held down at the time of the event.
```c#
bool HasShift { get; } 
```
WhetherShiftkey was being held down at the time of the event.
```c#
KeyboardModifiers KeyboardModifiers { get; set; } 
```
The keyboard modifier keys that were held down at the moment the event triggered.
```c#
Vector2 LocalPosition { get; set; } 
```
Cursor position, local to this widget.
