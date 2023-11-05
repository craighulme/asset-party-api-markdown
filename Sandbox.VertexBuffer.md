# VertexBuffer

## ```c#
Derives from object
```

## Summary

Whether this vertex buffer has any indexes. This is set byVertexBuffer.Init.
## Constructors

```c#
VertexBuffer( ) 
```
No Summary
## Fields

```c#
Vertex Default
```
No Summary
## Properties

```c#
bool Indexed { get; } 
```
Whether this vertex buffer has any indexes. This is set byVertexBuffer.Init.
## Methods

```c#
virtual void Clear( ) 
```
Clear all vertices and indices, and resetsVertexBuffer.Default.
```c#
virtual void Init( bool useIndexBuffer) 
```
Clear the buffer and set whether it will have indices.
```c#
void Add( Vertex v) 
```
Add a vertex
```c#
void AddIndex( int i) 
```
Add an index. This is relative to the top of the vertex buffer. So 0 is Vertex.Count., 1 is Vertex.Count -1
```c#
void AddRawIndex( int i) 
```
Add an index. This is NOT relative to the top of the vertex buffer.
```c#
void AddTriangleIndex( int a, int b, int c) 
```
Add a triangle by indices. This is relative to the top of the vertex buffer. So 0 is Vertex.Count.
## Extensions

```c#
void Add( Vector3 pos) 
```
Add a vertex using this position and everything else from Default
```c#
void Add( Vector3 pos, Vector2 uv) 
```
Add a vertex using this position and UV, and everything else from Default
```c#
void AddCube( Vector3 center, Vector3 size, Rotation rot, Color32 color = null) 
```
Add a cube to the vertex buffer. Will include indices if they're enabled.
```c#
void AddQuad( Rect rect) 
```
Add a quad to the vertex buffer. Will include indices if they're enabled.
```c#
void AddQuad( Vertex a, Vertex b, Vertex c, Vertex d) 
```
Add a quad to the vertex buffer. Will include indices if they're enabled.
```c#
void AddQuad( Vector3 a, Vector3 b, Vector3 c, Vector3 d) 
```
Add a quad to the vertex buffer. Will include indices if they're enabled.
```c#
void AddQuad( Ray origin, Vector3 width, Vector3 height) 
```
Add a quad to the vertex buffer. Will include indices if they're enabled.
```c#
void AddTriangle( Vertex a, Vertex b, Vertex c) 
```
Add a triangle to the vertex buffer. Will include indices if they're enabled.
```c#
void Draw( Material material, RenderAttributes attributes = null) 
```
Draw this mesh using Material
