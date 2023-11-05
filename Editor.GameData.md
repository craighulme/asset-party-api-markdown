# GameData

## ```c#
Derives from object
```

## Summary

Lets all native and managed tools know about any engine / game entities.
## Properties

```c#
static IReadOnlyList<MapClass> EntityClasses { get; } 
```
A list of all entity classes exposed to tools.
```c#
static Package[] LoadedPackages { get; set; } 
```
All loaded asset.party packages for this session to load entities for tools from.
## Methods

```c#
static Task LoadEntitiesFromPackage( Package package) 
```
Loads the entity classes from a remote asset.party game or addon into Hammer.
