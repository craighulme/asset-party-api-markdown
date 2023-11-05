# Entry

## 
```c#
Is interface
```

## Summary

A facet entry consists of a name, display information and the number of items inside
## Properties

```c#
abstract int Count { get; } 
```
The number of items within this facet
```c#
abstract string Icon { get; } 
```
The material icon for this facet
```c#
abstract string Name { get; } 
```
The name of this item. A filter for this would look like "facet.Name:facet.entry.Name"
```c#
abstract string Title { get; } 
```
The display name of this facet in English
