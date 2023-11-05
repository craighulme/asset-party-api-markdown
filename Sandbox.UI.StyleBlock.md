# StyleBlock

## ```c#
Implements IStyleBlock
```

## Summary

A CSS rule - ie ".chin { width: 100%; height: 100%; }"
## Constructors

```c#
StyleBlock( ) 
```
No Summary
## Fields

```c#
Styles Styles
```
The styles that are defined in this block
## Properties

```c#
virtual string AbsolutePath { get; } 
```
ImplementsIStyleBlock.AbsolutePathThe absolute on disk filename for this style block (or null if not on disk)
```c#
virtual int FileLine { get; } 
```
ImplementsIStyleBlock.FileLineThe line in the file containing this style block
```c#
virtual string FileName { get; } 
```
ImplementsIStyleBlock.FileNameThe filename of the file containing this style block (or null if none)
```c#
virtual IEnumerable<string> SelectorStrings { get; } 
```
ImplementsIStyleBlock.SelectorStringsA list of selectors for this block
```c#
StyleSelector[] Selectors { get; } 
```
A list of appropriate selectors for this block (ie ".button")
## Methods

```c#
virtual List<StyleProperty> GetRawValues( ) 
```
ImplementsIStyleBlock.GetRawValuesGet the list of raw style values
```c#
virtual void SetRawValue( string key, string value, string originalValue = null) 
```
ImplementsIStyleBlock.SetRawValueUpdate a raw style value
```c#
bool SetSelector( string selector, StyleBlock parent = null) 
```
No Summary
