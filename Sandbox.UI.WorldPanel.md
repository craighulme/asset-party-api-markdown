# WorldPanel

## ```c#
Derives from RootPanel
```

## Summary

An interactive 2D panel rendered in the 3D world.
## Constructors

```c#
WorldPanel( SceneWorld world = null) 
```
No Summary
## Properties

```c#
float MaxInteractionDistance { get; set; } 
```
Maximum distance at which a player can interact with this world panel.
```c#
Vector3 Position { get; set; } 
```
Position of the world panel in 3D space.
```c#
Rotation Rotation { get; set; } 
```
Rotation of the world panel in 3D space.
```c#
ScenePanelObject SceneObject { get; } 
```
Scene object that renders the panel.
```c#
Transform Transform { get; set; } 
```
Transform of the world panel in 3D space.
```c#
float WorldScale { get; set; } 
```
Scale of the world panel in 3D space.
## Methods

```c#
override void Delete( bool immediate = false) 
```
OverridesRootPanel.DeleteDeletes the panel.
```c#
override void OnDeleted( ) 
```
OverridesRootPanel.OnDeletedCalled when the panel is about to be deleted.
```c#
override bool RayToLocalPosition( Ray ray, out Vector2 position, out float distance) 
```
OverridesPanel.RayToLocalPositionTransform a ray in 3D space to a position on the panel. This is used for world panel input.
```c#
protected override void UpdateBounds( Rect rect) 
```
OverridesRootPanel.UpdateBoundsUpdate the bounds for this panel. We purposely do nothing here because
on world panels you can change the bounds by settingRootPanel.PanelBounds.
```c#
protected override void UpdateScale( Rect screenSize) 
```
OverridesRootPanel.UpdateScaleWe override this to prevent the scale automatically being set based on screen
size changing.. because that's obviously not needed here.
