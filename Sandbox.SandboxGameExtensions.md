# SandboxGameExtensions

## Is static
Derives from object

## Summary

Draw this mesh using Material
## Methods

```c#
static void Draw( VertexBuffer self, Material material, RenderAttributes attributes = null) 
```
Draw this mesh using Material
```c#
static T GetEntity<T,>( PhysicsBody self) 
```
Returns the entity this physics body belongs to.
```c#
static Entity GetEntity( PhysicsBody self) 
```
Returns the entity this physics body belongs to.
```c#
static bool IsMounted( Package package, bool downloadAndMount = false, bool withCode = false) 
```
Download and mount this package. If withCode is true we'll try to load the assembly if it exists.
```c#
static Task<BaseFileSystem> MountAsync( Package package) 
```
Download and mount this package.PAINDAY TODO: Delete me and makeSandboxGameExtensions.MountAsynchave an optional argument
```c#
static Task<BaseFileSystem> MountAsync( Package package, bool withCode) 
```
Download and mount this package. If withCode is true we'll try to load the assembly if it exists.
```c#
static Entity ReadEntity( BinaryReader reader) 
```
Read an entity from a binary reader.
```c#
static int ToPixels( InputGlyphSize size) 
```
Translates this enum to pixel size.
```c#
static Vector3 ToScreen( Vector3 self) 
```
Clientside, returns position of this 3D vector on local clients' screen in 2D coordinates based on theSandbox.Camera.
```c#
static Vector2? ToScreen( Vector3 self, Vector2 screenSize) 
```
Same asSandboxGameExtensions.ToScreen, but return value is in absolute coordinates.
```c#
static void Write( BinaryWriter writer, Entity ent) 
```
Write this entity to a binary writer.
