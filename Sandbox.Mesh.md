# Mesh

## ```c#
Derives from object
```

## Summary

Ameshis a basic version of aSandbox.Model,
containing a set of vertices and indices which make up faces that make up a shape.A set of meshes can be used to create aSandbox.Modelvia theSandbox.ModelBuilderclass.
## Constructors

```c#
Mesh( ) 
```
No Summary
```c#
Mesh( Material material, MeshPrimitiveType primType = 3) 
```
No Summary
## Properties

```c#
BBox Bounds { set; } 
```
Sets AABB bounds for this mesh.
```c#
bool HasIndexBuffer { get; } 
```
Whether this mesh has an index buffer.
```c#
bool HasVertexBuffer { get; } 
```
Whether this mesh has a vertex buffer.
```c#
int IndexCount { get; } 
```
Number of indices this mesh has.
```c#
bool IsValid { get; } 
```
Whether this object is valid or not.
```c#
Material Material { set; } 
```
Sets material for this mesh.
```c#
MeshPrimitiveType PrimitiveType { set; } 
```
Sets the primitive type for this mesh.
```c#
int VertexCount { get; } 
```
Number of vertices this mesh has.
## Methods

```c#
void CreateBuffers( VertexBuffer vb, bool calculateBounds = true) 
```
Create vertex and index buffers.
```c#
void CreateIndexBuffer( ) 
```
Create an empty index buffer, it can be resized later
```c#
void CreateIndexBuffer( int indexCount, List<int> data) 
```
Create a index buffer with a number of indices
```c#
void CreateIndexBuffer( int indexCount, Span<int> data = null) 
```
Create a index buffer with a number of indices
```c#
void CreateVertexBuffer<T,>( VertexAttribute[] layout) 
```
Create an empty vertex buffer, it can be resized later
```c#
void CreateVertexBuffer<T,>( int vertexCount, VertexAttribute[] layout, List<T> data) 
```
Create a vertex buffer with a number of vertices
```c#
void CreateVertexBuffer<T,>( int vertexCount, VertexAttribute[] layout, Span<T> data = null) 
```
Create a vertex buffer with a number of vertices
```c#
void LockIndexBuffer( IndexBufferLockHandler handler) 
```
Lock all the memory in this buffer so you can write to it
```c#
void LockIndexBuffer( int elementCount, IndexBufferLockHandler handler) 
```
Lock a specific amount of the memory in this buffer so you can write to it
```c#
void LockIndexBuffer( int elementOffset, int elementCount, IndexBufferLockHandler handler) 
```
Lock a region of memory in this buffer so you can write to it
```c#
void LockVertexBuffer<T,>( VertexBufferLockHandler<T> handler) 
```
Lock all the memory in this buffer so you can write to it
```c#
void LockVertexBuffer<T,>( int elementCount, VertexBufferLockHandler<T> handler) 
```
Lock a specific amount of the memory in this buffer so you can write to it
```c#
void LockVertexBuffer<T,>( int elementOffset, int elementCount, VertexBufferLockHandler<T> handler) 
```
Lock a region of memory in this buffer so you can write to it
```c#
void SetBounds( Vector3 mins, Vector3 maxs) 
```
Set the render bounds of this mesh, default is infinite
```c#
void SetIndexBufferData( List<int> data, int elementOffset = 0) 
```
Set data of this buffer
```c#
void SetIndexBufferData( Span<int> data, int elementOffset = 0) 
```
Set data of this buffer
```c#
void SetIndexBufferSize( int elementCount) 
```
Resize the index buffer.
```c#
void SetIndexRange( int start, int count) 
```
Set how many indices this mesh draws
```c#
void SetVertexBufferData<T,>( List<T> data, int elementOffset = 0) 
```
Set data of this buffer
```c#
void SetVertexBufferData<T,>( Span<T> data, int elementOffset = 0) 
```
Set data of this buffer
```c#
void SetVertexBufferSize( int elementCount) 
```
Resize the vertex buffer
```c#
void SetVertexRange( int start, int count) 
```
Set how many vertices this mesh draws (if there's no index buffer)
## Nested Types

