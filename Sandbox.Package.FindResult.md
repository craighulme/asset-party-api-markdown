# FindResult

## Is interface

## Summary

A result from the call to FindAsync
## Properties

```c#
abstract Facet[] Facets { get; } 
```
Facets particular to this search
```c#
abstract double Milliseconds { get; } 
```
The amount of time the query took
```c#
abstract SortOrder[] Orders { get; set; } 
```
A list of sort orders. There may be other sort orders, but we provide a list here that can
be easily used to save rewriting the same code over and over.
```c#
abstract Package[] Packages { get; } 
```
A list of packages retrieved
```c#
abstract TagEntry[] Tags { get; } 
```
A list of tags relevant to this search
```c#
abstract int TotalCount { get; } 
```
The total amount of packages
