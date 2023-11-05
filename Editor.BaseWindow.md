# BaseWindow

## ```c#
Derives from Widget
```

## Summary

OverridesWidget.OnClosedCalled when a window is closed.
## Constructors

```c#
BaseWindow( ) 
```
No Summary
## Properties

```c#
Action OnWindowClosed { get; set; } 
```
No Summary
## Methods

```c#
protected override void OnClosed( ) 
```
OverridesWidget.OnClosedCalled when a window is closed.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
override void SetWindowIcon( string name) 
```
OverridesWidget.SetWindowIcon
## Inheriting Types

