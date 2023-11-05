# Vertex

## Derives from ValueType

## Summary

No Summary
## Constructors

```c#
Vertex( Vector3 position) 
```
No Summary
```c#
Vertex( Vector3 position, Color32 color) 
```
No Summary
```c#
Vertex( Vector3 position, Vector4 texCoord0, Color32 color) 
```
No Summary
```c#
Vertex( Vector3 position, Vector3 normal, Vector3 tangent, Vector4 texCoord0) 
```
No Summary
## Fields

```c#
static readonly VertexAttribute[] Layout
```
No Summary
```c#
Color32 Color
```
No Summary
```c#
Vector3 Normal
```
No Summary
```c#
Vector3 Position
```
No Summary
```c#
Vector4 Tangent
```
No Summary
```c#
Vector4 TexCoord0
```
No Summary
```c#
Vector4 TexCoord1
```
No Summary
## Referencing Members

```c#
void VertexBuffer.Add( Vertex ) 
```
```c#
static void SandboxBaseExtensions.AddQuad( VertexBuffer, Vertex, Vertex, Vertex, Vertex ) 
```
```c#
static void SandboxBaseExtensions.AddTriangle( VertexBuffer, Vertex, Vertex, Vertex ) 
```
```c#
Vertex = VertexBuffer.Default
```
```c#
static void Graphics.Draw( Span<Vertex>, int, Material, RenderAttributes, PrimitiveType ) 
```
```c#
static void Graphics.Draw( List<Vertex>, int, Material, RenderAttributes, PrimitiveType ) 
```
```c#
static void Graphics.Draw( Span<Vertex>, int, Span<UInt16>, int, Material, RenderAttributes, PrimitiveType ) 
```
