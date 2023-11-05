# PrimitiveBuilder

## ```c#
Derives from object
```

## Summary

If this primitive is 2D the bounds box will be limited to have no depth.
## Constructors

```c#
protected PrimitiveBuilder( ) 
```
No Summary
## Properties

```c#
virtual bool Is2D { get; } 
```
If this primitive is 2D the bounds box will be limited to have no depth.
## Methods

```c#
virtual void Build( PolygonMesh mesh) 
```
Create the primitive in the mesh.
```c#
virtual void SetFromBox( BBox box) 
```
No Summary
