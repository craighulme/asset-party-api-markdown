# MapView

## Derives from object
Implements IHandle

## Summary

MapViews are owned by the MapViewMgr. They display the MapViewMgr's mapdoc.The MapView provides either a 2d or 3d view of the provided map doc. The rendering mode
may be swapped between various 2d and 3d modes dynamically. In addition to basic display
functionality the view also provides movement implementation for moving a camera within a 3d view
or panning a 2d view.
## Properties

```c#
Instance GizmoInstance { get; set; } 
```
No Summary
```c#
MapDocument MapDoc { get; } 
```

```c#
Vector2 MousePosition { get; } 
```

```c#
SceneCamera SceneCamera { get; init; } 
```
Read-only SceneCamera set automatically during rendering
## Methods

```c#
void BuildRay( out Vector3 startRay, out Vector3 endRay) 
```
Builds a ray from the mouse cursor
