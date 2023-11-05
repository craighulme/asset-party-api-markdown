# DebugOverlay

## ```c#
Derives from object
```

## Summary

Overlays to show useful information whilst debugging.
## Constructors

```c#
DebugOverlay( ) 
```
No Summary
## Methods

```c#
void Axis( Vector3 position, Rotation rotation, float length = 10, float duration = 0, bool depthTest = true) 
```
Draw a 3D Axis representation in 3D
```c#
void Box( Vector3 mins, Vector3 maxs) 
```
Draw an axis aligned yellow box in 3D space for 1 frame
```c#
void Box( Vector3 mins, Vector3 maxs, Color color, float duration = 0, bool depthTest = true) 
```
Draw an axis aligned box in 3D space
```c#
void Box( Vector3 position, Vector3 mins, Vector3 maxs, Color color, float duration = 0, bool depthTest = true) 
```
Draw an axis aligned box in 3D space
```c#
void Box( Vector3 position, Rotation rotation, Vector3 mins, Vector3 maxs, Color color, float duration = 0, bool depthTest = true) 
```
Draw a rotated box in 3D space
```c#
void Box( Entity ent, Color color, float duration = 0) 
```
Draw orientated bounds of an entity.
```c#
void Box( PhysicsBody body, Color color, float duration = 0) 
```
Draw axis aligned bounds of a physics body.
```c#
void Box( BBox bounds, Color color, float duration = 0) 
```
Visualize given AABB.
```c#
void Circle( Vector3 position, Rotation rotation, float radius, Color color, float duration = 0, bool depthTest = true) 
```
Render a flat circle in 3D space
```c#
void Line( Vector3 start, Vector3 end, Color color, float duration = 0, bool depthTest = true) 
```
Draw a line in 3D space
```c#
void Line( Vector3 start, Vector3 end, float duration = 0, bool depthTest = true) 
```
Draw a yellow line in 3D space
```c#
void ScreenText( string text, Vector2 position, int line, Color color, float duration = 0) 
```
Draw 2D text
```c#
void ScreenText( string text, Vector2 position, float duration = 0) 
```
Draw yellow 2D text
```c#
void ScreenText( string text, int line = 0, float duration = 0) 
```
Draw yellow 2D text @ {100, 100}
```c#
bool Skeleton( Entity ent, Color color, float duration = 0, bool depthTest = true) 
```
Draw this entity's skeleton (if it has one)
```c#
void Sphere( Vector3 position, float radius, Color color, float duration = 0, bool depthTest = true) 
```
Render a sphere in 3D space
```c#
void Sphere( Sphere sphere, Color color, float duration = 0) 
```
Visualize a given sphere.
```c#
void Text( string text, Vector3 pos, int offset, Color color, float duration = 0, float maxDistance = 1500) 
```
Draw text in 3D space
```c#
void Text( string text, Vector3 pos, Color color, float duration = 0, float maxDistance = 1500) 
```
Draw text in 3D space
```c#
void Text( string text, Vector3 pos, float duration = 0, float maxDistance = 1500) 
```
Draw yellow text in 3D space
```c#
void Texture( Texture texture, Vector2 position, float duration = 0) 
```
Render a 2D texture
```c#
void Texture( Texture texture, Rect rect, float duration = 0) 
```
Render a 2D texture
```c#
void Texture( Texture texture, Rect rect, Color color, Vector2 topLeftUV, Vector2 bottomRightUV, float duration = 0) 
```
Render a 2D texture
```c#
void TraceResult( TraceResult tr, float duration = 0) 
```
Visualize a trace
