# StyleSheetCollection

## 
```c#
Derives from ValueType
```

## Summary

A collection ofUI.StyleSheetobjects applied directly to a panel.
SeePanel.StyleSheet.
## Methods

```c#
void Add( StyleSheet sheet) 
```
Add a stylesheet directly
```c#
IEnumerable<ValueTuple<string, string>> CollectVariables( ) 
```
Returns all CSS variables from the owning panel and its ancestors.
```c#
void Load( string filename, bool inheritVariables = true) 
```
Load the stylesheet from a file.
```c#
void Parse( string stylesheet, bool inheritVariables = true) 
```
Load the stylesheet from a string.
```c#
void Remove( StyleSheet sheet) 
```
Remove a specificUI.StyleSheetfrom the collection.
```c#
void Remove( string wildcardGlob) 
```
Remove all stylesheets whose filename matches this wildcard glob.
## Referencing Members

```c#
StyleSheetCollection = Panel.StyleSheet
```
