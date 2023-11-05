# NoticeWidget

## ```c#
Derives from Widget
```

## Summary

Called when it's about to be re-used by a new compiler
## Constructors

```c#
NoticeWidget( ) 
```
No Summary
## Fields

```c#
Color BorderColor
```
No Summary
```c#
bool DrawTimer
```
No Summary
```c#
string Icon
```
No Summary
```c#
bool IsRunning
```
No Summary
```c#
float ProgressDelta
```
No Summary
```c#
string Subtitle
```
No Summary
```c#
string Title
```
No Summary
## Properties

```c#
virtual bool WantsVisible { get; } 
```
No Summary
## Methods

```c#
virtual void Reset( ) 
```
Called when it's about to be re-used by a new compiler
```c#
virtual void Tick( ) 
```
No Summary
```c#
void SetBodyWidget( Widget body) 
```
Set a body widget to which the notice will stretch
```c#
protected override void OnMousePress( MouseEvent e) 
```
OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
