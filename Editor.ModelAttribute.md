# ModelAttribute

## 
```c#
Derives from Attribute
```

## Summary

This makes it so the model, skin and bodygroups can be set and changed in Hammer.
## Constructors

```c#
ModelAttribute( ) 
```
No Summary
## Properties

```c#
ModelArchetype Archetypes { get; set; } 
```
Marks this entity as a representative of a certain model archetype.
This makes this entity class appear in ModelDoc under given archetype(s), which will be used to decide which entity class to use when dragging models from Hammer's Asset browser.
```c#
string BodyGroup { get; set; } 
```
The default body group to be set to.
```c#
string MaterialGroup { get; set; } 
```
The default material group to be set to.
```c#
string Model { get; set; } 
```
The default model to be set to.
