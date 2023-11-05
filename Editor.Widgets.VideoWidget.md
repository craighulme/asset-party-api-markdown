# VideoWidget

## ```c#
Derives from Widget
```

## Summary

A widget that uses a pixmap to display a video.
## Constructors

```c#
VideoWidget( Widget parent, string url) 
```
No Summary
## Properties

```c#
VideoPlayer Player { get; } 
```
Access to the video player to control playback.
## Methods

```c#
void Frame( ) 
```
No Summary
```c#
override void OnDestroyed( ) 
```
OverridesQObject.OnDestroyed
```c#
protected override void OnMouseClick( MouseEvent e) 
```
OverridesWidget.OnMouseClickCalled when this widget is left clicked (on mouse release).
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
