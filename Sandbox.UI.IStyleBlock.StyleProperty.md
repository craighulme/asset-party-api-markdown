# StyleProperty

## ```c#
Derives from ValueType
```

## Summary

The line in the file containing this value
## Properties

```c#
int Line { get; set; } 
```
The line in the file containing this value
```c#
string Name { get; set; } 
```
Name of the property, ie "color" or "width"
```c#
string OriginalValue { get; set; } 
```
The value that was loaded from the .scss file
```c#
string Value { get; set; } 
```
Current value of the property (which is being rendered)
## Referencing Members

```c#
abstract List<StyleProperty> = IStyleBlock.GetRawValues( ) 
```
```c#
virtual List<StyleProperty> = StyleBlock.GetRawValues( ) 
```
