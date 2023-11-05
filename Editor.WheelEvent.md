# WheelEvent

## 
```c#
Derives from ValueType
```

## Summary

Information about a mouse wheel scroll event of aEditor.Widget.
## Properties

```c#
float Delta { get; } 
```
No Summary
```c#
Vector2 GlobalPosition { get; } 
```
No Summary
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
Vector2 Position { get; } 
```
No Summary
## Methods

```c#
void Accept( ) 
```
No Summary
```c#
void Ignore( ) 
```
No Summary
## Referencing Members

```c#
protected override void BaseScrollWidget.OnWheel( WheelEvent ) 
```
```c#
protected virtual void Widget.OnWheel( WheelEvent ) 
```
```c#
protected override void AssetList.OnWheel( WheelEvent ) 
```
```c#
protected override void WebWidget.OnWheel( WheelEvent ) 
```
```c#
protected override void GraphView.OnWheel( WheelEvent ) 
```
```c#
protected override void AssetPreviewWidget.OnWheel( WheelEvent ) 
```
```c#
protected override void TimelineView.OnWheel( WheelEvent ) 
```
