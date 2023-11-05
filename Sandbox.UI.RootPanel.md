# RootPanel

## 
```c#
Derives from Panel
```

## Summary

A root panel. Serves as a container for other panels, handles things such as rendering.
## Constructors

```c#
RootPanel( ) 
```
No Summary
## Properties

```c#
virtual bool IsWorldPanel { get; } 
```
True if this is a world panel, so should be skipped when determining cursor visibility etc
```c#
bool IsHighQualityVR { get; } 
```
If this panel should be rendered with ~4K resolution.
```c#
bool IsVR { get; } 
```
If this panel belongs to aSandbox.VROverlay.
```c#
Rect PanelBounds { get; set; } 
```
Bounds of the panel, i.e. its size and position on the screen.
```c#
bool RenderedManually { get; set; } 
```
If set to true this panel won't be rendered to the screen like a normal panel.
This is true when the panel is drawn via other means (like as a world panel)
```c#
float Scale { get; protected set; } 
```
The scale of this panel and its children.
## Methods

```c#
protected virtual void UpdateBounds( Rect rect) 
```
Called before layout to lock the bounds of this root panel to the screen size (which is passed).
Internally this sets PanelBounds to rect and calls UpdateScale.
```c#
protected virtual void UpdateScale( Rect screenSize) 
```
Work out scaling here. Default is to scale relative to the screen being
1920 wide. ie - scale = screensize.Width / 1920.0f;
```c#
void RenderManual( float opacity = 1) 
```
Render this panel manually. This gives more flexibility to where UI is rendered, to texture for example.RootPanel.RenderedManuallymust be set to true.
```c#
override void Delete( bool immediate = true) 
```
OverridesPanel.DeleteDeletes the panel.
```c#
override void OnDeleted( ) 
```
OverridesPanel.OnDeletedCalled when the panel is about to be deleted.
```c#
override void OnLayout( ref Rect layoutRect) 
```
OverridesPanel.OnLayoutThis panel has just been laid out. You can modify its position now and it will affect its children.
This is a useful place to restrict shit to the screen etc.
## Inheriting Types

