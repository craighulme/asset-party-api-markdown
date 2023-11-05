# ComputeShader

## Derives from object

## Summary

Dispatch this compute shader. This can be called outside of a graphics context.
## Constructors

```c#
ComputeShader( string computeShader) 
```
No Summary
```c#
ComputeShader( Material material) 
```
No Summary
## Properties

```c#
RenderAttributes Attributes { get; } 
```
No Summary
## Methods

```c#
void Dispatch( int threadsX = 32, int threadsY = 32, int threadZ = 32) 
```
Dispatch this compute shader. This can be called outside of a graphics context.
