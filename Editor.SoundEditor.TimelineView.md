# TimelineView

## 
```c#
Derives from GraphicsView
```

## Summary

OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
## Constructors

```c#
TimelineView( Timeline parent) 
```
No Summary
## Properties

```c#
float Duration { get; } 
```
No Summary
```c#
bool Scrubbing { get; set; } 
```
No Summary
```c#
string Sound { get; } 
```
No Summary
```c#
int SoundHandle { get; } 
```
No Summary
```c#
float Time { get; set; } 
```
No Summary
```c#
float ZoomFactor { get; } 
```
No Summary
## Methods

```c#
void MoveScrubber( float position) 
```
No Summary
```c#
void OnFrame( ) 
```
No Summary
```c#
float PositionFromTime( float time) 
```
No Summary
```c#
void SetPhonemes( List<PhonemeFrame> frames) 
```
No Summary
```c#
void SetSamples( Int16[] samples, float duration, string sound) 
```
No Summary
```c#
float TimeFromPosition( float position) 
```
No Summary
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
protected override void OnContextMenu( ContextMenuEvent e) 
```
OverridesWidget.OnContextMenuCalled afterWidget.OnMouseRightClick, for the purposes of opening a context menu.
```c#
override void OnDestroyed( ) 
```
OverridesQObject.OnDestroyed
```c#
protected override void OnWheel( WheelEvent e) 
```
OverridesWidget.OnWheelMouse wheel was scrolled while the mouse cursor was over this widget.
