# IconAttribute

## ```c#
Implements IIconProvider, IUninheritable
```

## Summary

Sets the icon of a type or a type member. Colors are expected in HTML formats, like "rgb(255,255,255)" or "#FFFFFF".
This info can then be retrieved via DisplayInfo library.
## Constructors

```c#
IconAttribute( string icon, string bgColor, string fgColor) 
```
No Summary
```c#
IconAttribute( string icon) 
```
No Summary
## Properties

```c#
Color? BackgroundColor { get; } 
```
The preferred background color for the icon.
```c#
Color? ForegroundColor { get; } 
```
The preferred color of the icon itself.
```c#
string Value { get; set; } 
```
ImplementsIIconProvider.ValueThe icon. Typically this is the name of amaterial icon.
