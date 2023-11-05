# BaseResourceEditor<T>

## 
```c#
Derives from Widget
```

## Summary

Implement this with your target type to create a special inspector for the resource type
See Editor.ClothingEditor for a cromulent example of this.
## Type Parameters

```c#
T is Resource, 
```
No Summary
## Constructors

```c#
BaseResourceEditor( ) 
```
Default constructor does nothing
## Properties

```c#
Asset Asset { get; } 
```
The asset we're editing
```c#
T Resource { get; } 
```
The resource contained within the asset
## Methods

```c#
protected abstract void Initialize( Asset asset, T resource) 
```
Override this to build your UI or whatever for this. Default behaviour is to
create a property sheet and add it to y
