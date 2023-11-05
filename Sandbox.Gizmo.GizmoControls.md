# GizmoControls

## ```c#
Derives from object
```

## Summary

Extendable helper to create common gizmos
## Methods

```c#
static IDisposable PushFixedScale( float? scale = null) 
```
Scope this before drawing a control to obey Settings.GimzoScale
```c#
bool Arrow( string name, Vector3 axis, out float distance, float length = 24, float girth = 6, float axisOffset = 2, float cullAngle = 10, float snapSize = 0, string head = "cone") 
```
Draw an arrow - return move delta if interacted with
```c#
bool DragSquare( string name, Vector2 size, Rotation rotation, out Vector3 movement, Action drawHandle = null) 
```
Manipulate a 2d value by moving on 2 axis
```c#
bool Position( string name, Vector3 position, out Vector3 newPos, Rotation? axisRotation = null, float squareSize = 3) 
```
A front left up position movement widget. If widget was moved then will return true and out will return the new position.
```c#
bool Rotate( string name, Angles value, out Angles newValue) 
```
A full rotation gizmo. If rotated will return true and newValue will be the new value
```c#
bool Rotate( string name, Rotation value, out Rotation outValue) 
```
A full rotation gizmo. If rotated will return true and newValue will be the new value
```c#
bool RotateSingle( string name, Rotation rotation, Color color, out Rotation delta, float size = 18) 
```
A single rotation axis
```c#
bool Scale( string name, float value, out float outValue) 
```
A front left up position movement widget. If widget was moved then will return true and out will return the new position.
