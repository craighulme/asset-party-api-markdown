# Image

## Derives from Panel

## Summary

A generic box that displays a given texture within itself.
## Constructors

```c#
Image( ) 
```
No Summary
## Properties

```c#
Texture Texture { get; set; } 
```
The texture being displayed by this panel.
```c#
override bool HasContent { get; } 
```
OverridesPanel.HasContentIf true, callsPanel.DrawContent.
## Methods

```c#
void SetTexture( string name) 
```
SetImage.Texturefrom a file path. URLs supported.
```c#
override void SetProperty( string name, string value) 
```
OverridesPanel.SetPropertySet a property on the panel, such as special properties (class,id,styleandvalue, etc.) and properties of the panel's C# class.
