# CanDropAttribute

## Derives from Attribute
Implements ITypeAttribute

## Summary

Can drop aSandbox.Packageof this type.
## Constructors

```c#
CanDropAttribute( Type packageType) 
```
Can drop aSandbox.Packageof this type.
```c#
CanDropAttribute( string assetFileExtension) 
```
Can drop aEditor.Assetof this file extension.
## Properties

```c#
virtual Type TargetType { get; set; } 
```
ImplementsITypeAttribute.TargetTypeThe type this attribute was attached to.
```c#
string AssetFileExtension { get; init; } 
```
No Summary
```c#
Type PackageType { get; init; } 
```
No Summary
