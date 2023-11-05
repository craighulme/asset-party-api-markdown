# Trace

## ```c#
Derives from ValueType
```

## Summary

Trace for tools, not to be confused with Sandbox.Trace
## Methods

```c#
static Trace Ray( in Vector3 from, in Vector3 to) 
```
Create a trace ray.
```c#
Trace MeshesOnly( ) 
```
Only trace against hammer mesh geometry ( CMapMesh nodes )
```c#
TraceResult Run( MapWorld world) 
```
Runs a trace against given world.
```c#
Trace SkipToolsMaterials( ) 
```
Don't hit tools materials (materials with thetools.toolsmaterialattribute)
