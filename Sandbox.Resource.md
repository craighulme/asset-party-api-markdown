# Resource

## 
```c#
Derives from object
```

## Summary

A resource loaded in the engine, such as aSandbox.ModelorSandbox.Material.
## Constructors

```c#
Resource( ) 
```
No Summary
## Properties

```c#
bool IsPromise { get; protected set; } 
```
Whether this resource was NOT loaded from disk, but rather simply contains the target filepath on disk.
This can happen for assets that don't exist.
```c#
int ResourceId { get; protected set; } 
```
ID of this resource,
```c#
string ResourceName { get; protected set; } 
```
File name of the resource without the extension.
```c#
string ResourcePath { get; protected set; } 
```
Path to this resource.
## Inheriting Types

