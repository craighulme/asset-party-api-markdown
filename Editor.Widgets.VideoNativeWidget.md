# VideoNativeWidget

## ```c#
Derives from NativeRenderingWidget
```

## Summary

A widget that uses native rendering to display a video.
## Constructors

```c#
VideoNativeWidget( Widget parent, string url) 
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
ImplementsNativeRenderingWidget.Frame
```c#
override void OnDestroyed( ) 
```
OverridesQObject.OnDestroyed
```c#
protected override void OnMouseClick( MouseEvent e) 
```
OverridesWidget.OnMouseClickCalled when this widget is left clicked (on mouse release).
```c#
protected override void OnResize( ) 
```
OverridesWidget.OnResizeCalled when the widgets' size was changed.
