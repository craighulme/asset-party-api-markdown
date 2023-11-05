# GameResourceAttribute

## 
```c#
Implements ITypeAttribute, IUninheritable
```

## Summary

Should be applied to a class that inherits fromSandbox.GameResource.
Makes the class able to be stored as an asset on disk.
## Constructors

```c#
GameResourceAttribute( string title, string extension, string description) 
```
No Summary
## Properties

```c#
virtual Type TargetType { get; set; } 
```
ImplementsITypeAttribute.TargetTypeThe type this attribute was attached to.
```c#
string Category { get; set; } 
```
Category of this game resource, for grouping in UI.
```c#
string Description { get; set; } 
```
Description of this game resource.
```c#
string Extension { get; set; } 
```
File extension for this game resource.
```c#
string Icon { get; set; } 
```
Icon to be used for this asset
Can be an absolute path of a PNG
Or amaterial iconfor this game resource's thumbnail.
```c#
string IconBgColor { get; set; } 
```
Background color for this resource's thumbnail.
```c#
string IconFgColor { get; set; } 
```
Foreground color (icon color) for this resource's thumbnail.
```c#
string Name { get; set; } 
```
The title of this game resource.
