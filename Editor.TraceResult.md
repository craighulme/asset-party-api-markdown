# TraceResult

## 
```c#
Derives from ValueType
```

## Summary

Whether the trace hit something or not
## Fields

```c#
bool Hit
```
Whether the trace hit something or not
```c#
Vector3 HitPosition
```
The hit position of the trace
```c#
MapNode MapNode
```
The map node that was hit, if any
```c#
Vector3 Normal
```
The hit surface normal (direction vector)
## Referencing Members

```c#
TraceResult = Trace.Run( MapWorld ) 
```
