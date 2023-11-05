# PopupWidget

## ```c#
Derives from Widget
```

## Summary

A popup widget that automatically deletes itself once it stops being visible
## Constructors

```c#
PopupWidget( Widget widget) 
```
No Summary
## Methods

```c#
void AddShadow( ) 
```
Add a shadow underneath this popup. This should be called BEFORE you make your
popup visible.
```c#
void OpenAt( Vector2 position, bool animate = true, Vector2? animateOffset = null) 
```
No Summary
```c#
void OpenAtCursor( bool animate = true, Vector2? offset = null) 
```
No Summary
```c#
void OpenBelowCursor( float distance, float centering = 0.5) 
```
Open the window this many pixels below the cursor.
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
protected override void OnMoved( ) 
```
OverridesWidget.OnMovedCalled when the widget was moved.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override void OnResize( ) 
```
OverridesWidget.OnResizeCalled when the widgets' size was changed.
```c#
protected override void OnVisibilityChanged( bool visible) 
```
OverridesWidget.OnVisibilityChangedCalled when the visibility of this widget changes.
## Inheriting Types

