# GameResource

## ```c#
Derives from Resource
```

## Summary

Assets defined in C# and created through tools.
You can define your ownCustom Asset Types.
## Constructors

```c#
protected GameResource( ) 
```
No Summary
## Methods

```c#
protected virtual void PostLoad( ) 
```
Called when the asset is first loaded from disk.
```c#
protected virtual void PostReload( ) 
```
Called when the asset is recompiled/reloaded from disk.
```c#
IEnumerable<string> GetReferencedPackages( ) 
```
Get a list of packages that are needed to load this asset
## Inheriting Types

