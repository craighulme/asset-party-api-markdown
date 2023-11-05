# IStyleBlock

## ```c#
Is interface
```

## Summary

A CSS rule - ie ".chin { width: 100%; height: 100%; }"
## Properties

```c#
abstract string AbsolutePath { get; } 
```
The absolute on disk filename for this style block (or null if not on disk)
```c#
abstract int FileLine { get; } 
```
The line in the file containing this style block
```c#
abstract string FileName { get; } 
```
The filename of the file containing this style block (or null if none)
```c#
abstract IEnumerable<string> SelectorStrings { get; } 
```
A list of selectors
## Methods

```c#
abstract List<StyleProperty> GetRawValues( ) 
```
Get the list of raw style values
```c#
abstract void SetRawValue( string key, string value, string originalValue = null) 
```
Update a raw style value
## Nested Types

