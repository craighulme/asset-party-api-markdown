# Facet

## Is interface

## Summary

Describes a facet of a group of items, with a limited
number of each facet with their total item counts
## Properties

```c#
abstract Entry[] Entries { get; } 
```
A list of entries inside this facet.
```c#
abstract string Name { get; } 
```
The internal name of this facet. This is used to reference the facet in filters.
```c#
abstract string Title { get; } 
```
The print friendly title of this facet in English.
## Nested Types

