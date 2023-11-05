# BBox

## 
```c#
Implements IEquatable<BBox>
```

## Summary

AnAxis Aligned Bounding Box.
PAIN DAY TODO: We should probably name this better. BoundingBox, AxisAlignedBoundingBox, or something else. AxisAlignedBounds?
## Constructors

```c#
BBox( Vector3 mins, Vector3 maxs) 
```
Initialize an AABB with given mins and maxs corners. SeeVector3.Sort.
```c#
BBox( Vector3 center, float size = 0) 
```
Initializes a zero sized BBox with given center. This is useful if you intend to use AddPoint to expand the box later.
## Fields

```c#
Vector3 Maxs
```
The maximum corner extents of the AABB. Values on each axis should be mathematically larger than values on the same axis ofBBox.Mins. SeeVector3.Sort
```c#
Vector3 Mins
```
The minimum corner extents of the AABB. Values on each axis should be mathematically smaller than values on the same axis ofBBox.Maxs. SeeVector3.Sort
## Properties

```c#
Vector3 Center { get; } 
```
Calculated center of the AABB.
```c#
IEnumerable<Vector3> Corners { get; } 
```
An enumerable that contains all corners of this AABB.
```c#
Vector3 RandomPointInside { get; } 
```
Returns a random point within this AABB.
```c#
Vector3 Size { get; } 
```
Calculated size of the AABB on each axis.
```c#
float Volume { get; } 
```
Returns the physical volume of this AABB.
## Methods

```c#
static BBox FromBoxes( IEnumerable<BBox> boxes) 
```
Create a bounding box from an arbituary number of other boxes
```c#
static BBox FromHeightAndRadius( float height, float radius) 
```
Creates an AABB ofradiuslength and depth, and givenheight
```c#
static BBox FromPoints( IEnumerable<Vector3> points, float size = 0) 
```
Create a bounding box from an arbituary number of points
```c#
static BBox FromPositionAndSize( Vector3 center, float size) 
```
Creates an AABB at given positioncenterand givensizewhich acts as adiameterof a sphere contained within the AABB.
```c#
static BBox FromPositionAndSize( Vector3 center, Vector3 size) 
```
Creates an AABB at given positioncenterand givensizea.k.a. "extents".
```c#
BBox AddBBox( in BBox point) 
```
Returns this bbox but stretched to include given bbox
```c#
BBox AddPoint( Vector3 point) 
```
Returns this bbox but stretched to include given point
```c#
Vector3 ClosestPoint( Vector3 point) 
```
Returns the closest point on this AABB to another point
```c#
bool Contains( BBox b) 
```
Returns true if this AABB completely contains given AABB
```c#
bool Contains( Vector3 b) 
```
Returns true if this AABB contains given point
```c#
bool Overlaps( BBox b) 
```
Returns true if this AABB somewhat overlaps given AABB
```c#
BBox Rotate( Rotation rotation) 
```
Rotate this box by this amount and return
```c#
bool Trace( Ray ray, float distance, out float hitDistance) 
```
Trace a ray against this box. If hit then return the distance.
```c#
BBox Transform( Transform transform) 
```
Transform this box by this amount and return
```c#
BBox Translate( Vector3 point) 
```
Move this box by this amount and return
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( BBox o) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
```c#
override string ToString( ) 
```
OverridesValueType.ToStringFormats this AABB into a string "mins x,y,z, maxs x,y,z"
## Operators

```c#
BBox +( BBox c1, Vector3 c2) 
```
No Summary
```c#
bool ==( BBox left, BBox right) 
```
No Summary
```c#
bool !=( BBox left, BBox right) 
```
No Summary
```c#
BBox *( BBox c1, float c2) 
```
No Summary
## Referencing Members

```c#
void GizmoHitbox.BBox( BBox ) 
```
```c#
BBox = SceneFogVolume.BoundingBox { get; set; } 
```
```c#
BBox = Node.BoundingBox { get; } 
```
```c#
BBox = Mesh.Bounds { set; } 
```
```c#
BBox = Model.Bounds { get; } 
```
```c#
BBox = SceneMap.Bounds { get; } 
```
```c#
BBox = SceneObject.Bounds { get; set; } 
```
```c#
BBox = HullPart.Bounds { get; init; } 
```
```c#
BBox = MeshPart.Bounds { get; init; } 
```
```c#
PhysicsTraceBuilder = PhysicsTraceBuilder.Box( BBox, in Vector3, in Vector3 ) 
```
```c#
PhysicsTraceBuilder = PhysicsTraceBuilder.Box( BBox, in Ray, in float ) 
```
```c#
static Trace = Trace.Box( BBox, in Vector3, in Vector3 ) 
```
```c#
static Trace = Trace.Box( BBox, in Ray, in float ) 
```
```c#
void DebugOverlay.Box( BBox, Color, float ) 
```
```c#
BBox = ModelEntity.CollisionBounds { get; set; } 
```
```c#
static Model = PlanarReflection.CreateBoundingMeshModel( BBox ) 
```
```c#
static IEnumerable<Entity> = Entity.FindInBox( BBox ) 
```
```c#
BBox = Frustum.GetBBox( ) 
```
```c#
BBox = PhysicsBody.GetBounds( ) 
```
```c#
virtual BBox = BasePlayerController.GetHull( ) 
```
```c#
override BBox = WalkController.GetHull( ) 
```
```c#
bool = Plane.IsInFront( BBox, bool ) 
```
```c#
bool = Frustum.IsInside( BBox, bool ) 
```
```c#
BBox = SceneObject.LocalBounds { get; set; } 
```
```c#
BBox = Model.PhysicsBounds { get; } 
```
```c#
PlanarReflection.PlanarReflection( SceneWorld, BBox ) 
```
```c#
BBox = SceneCubemap.ProjectionBounds { get; set; } 
```
```c#
BBox = Model.RenderBounds { get; } 
```
```c#
BBox = RenderEntity.RenderBounds
```
```c#
SceneCubemap.SceneCubemap( SceneWorld, Texture, BBox ) 
```
```c#
SceneFogVolume.SceneFogVolume( SceneWorld, Transform, BBox, float, float ) 
```
```c#
virtual void PrimitiveBuilder.SetFromBox( BBox ) 
```
```c#
void GizmoDraw.SolidBox( BBox ) 
```
```c#
abstract BBox = IEntity.WorldSpaceBounds { get; } 
```
```c#
virtual BBox = Entity.WorldSpaceBounds { get; } 
```
