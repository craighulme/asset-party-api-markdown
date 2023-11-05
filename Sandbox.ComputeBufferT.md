# ComputeBuffer<T>

## 
```c#
Implements IDisposable
```

## Summary

A GPU data buffer intended for use with aSandbox.ComputeShader.You can read and write arbitrary data to and from the CPU and GPU.
This allows for efficient parallel data processing on the GPU.Different GPU buffer types can be used depending on the providedSandbox.ComputeBufferType.
Using the defaultComputeBufferType.Structuredtype buffers map to StructuredBuffer<T> and RWStructuredBuffer<T> in HLSL.
## Type Parameters

```c#
T is ValueType, new(), 
```
No Summary
## Constructors

```c#
ComputeBuffer( int elementCount, ComputeBufferType type = 0) 
```
Creates a new GPU buffer with a specified number of elements and a specific buffer type.
## Methods

```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.DisposeDestroys the GPU buffer, don't use it no more
```c#
void CopyStructureCount<U,>( ComputeBuffer<U> destBuffer, int destBufferOffset) 
```
No Summary
```c#
void GetData( Span<T> data) 
```
Retrieves the GPU buffer and copies them into a provided Span.
```c#
void GetData( Span<T> data, int start, int count) 
```
Retrieves a number of elements from the GPU buffer and copies them into a provided Span.
```c#
void SetData( List<T> data, int elementOffset = 0) 
```
Synchronously uploads data from a List to the GPU, replacing the existing data in this ComputeBuffer.
```c#
void SetData( Span<T> data, int elementOffset = 0) 
```
Synchronously uploads data from a Span to the GPU, replacing the existing data in this ComputeBuffer.
