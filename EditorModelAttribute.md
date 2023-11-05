# EditorModelAttribute

## ```c#
Derives from Attribute
```

## Summary

Declare a model to represent this entity in editor. This is a common attribute so it's leaked out of the Editor namespace.
## Constructors

```c#
EditorModelAttribute( string model, string staticColor = "white", string dynamicColor = "white") 
```
No Summary
## Properties

```c#
bool CastShadows { get; set; } 
```
Whether the model should cast shadows in the editor.
```c#
Color DynamicColor { get; set; } 
```
Tint color for this editor model instance when the entity it represents is dynamic.
```c#
bool FixedBounds { get; set; } 
```
Don't reorient bounds. This is used for things that have fixed bounds in the game, like info_player_start.
```c#
string Model { get; set; } 
```
The model to display in the editor.
```c#
Color StaticColor { get; set; } 
```
Tint color for this editor model instance when the entity it represents is static.
