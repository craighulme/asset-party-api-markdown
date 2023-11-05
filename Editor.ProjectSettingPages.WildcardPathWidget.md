# WildcardPathWidget

## 
```c#
Derives from Widget
```

## Summary

These paths will be collapsed so that files look like they're in the root
## Constructors

```c#
WildcardPathWidget( Widget parent) 
```
No Summary
## Properties

```c#
string[] CollapsePaths { get; set; } 
```
These paths will be collapsed so that files look like they're in the root
```c#
DirectoryInfo Directory { set; } 
```
No Summary
```c#
bool HideAssets { get; set; } 
```
Hide all assets. That is to say, hide all files that compile into something. We
do this on the resources tab because all of the compiled files are included anyway!
```c#
string[] IgnoreFiles { get; } 
```
A list of wildcard files that we don't even want to show here
```c#
string Value { get; set; } 
```
No Summary
## Methods

```c#
void Frame( ) 
```
No Summary
