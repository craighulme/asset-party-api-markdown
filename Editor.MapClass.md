# MapClass

## ```c#
Derives from object
```

## Summary

Represents an entity class used by the map editor
## Constructors

```c#
MapClass( string name) 
```
No Summary
## Properties

```c#
string Category { get; } 
```
Category
```c#
string Description { get; } 
```
Human readable name e.g Physics Prop
```c#
string DisplayName { get; } 
```
Display name e.g Physics Prop
```c#
List<Tuple<string, string[]>> EditorHelpers { get; } 
```
In-editor helpers for this class, such as box visualizers for certain properties, etc.
```c#
string GameIdent { get; } 
```
What game does this belong to? ( TODO: Might not be best place for this? )
```c#
string Icon { get; } 
```
Icon ( Material )
```c#
List<Input> Inputs { get; } 
```
List of inputs for this class.
```c#
bool IsCableClass { get; } 
```
A cable entity, will appear in the Path Tool.
```c#
bool IsPathClass { get; } 
```
A path entity, will appear in the Path Tool.
```c#
bool IsPointClass { get; } 
```
A point entity, i.e. a model entity, etc.
```c#
bool IsSolidClass { get; } 
```
A solid class entity, triggers, etc., entities that are tied to from a mesh in Hammer
```c#
Dictionary<string, object> Metadata { get; } 
```
General purpose key-value store to alter functionality of UI, map compilation, editor helpers, etc.
```c#
string Name { get; } 
```
Class name e.g prop_physics
```c#
List<Output> Outputs { get; } 
```
List of outputs for this class.
```c#
Package Package { get; } 
```
What package did this entity come from?
```c#
List<string> Tags { get; } 
```
General purpose tags, some with special meanings within Hammer and map compilers.
```c#
Type Type { get; } 
```
C# Type of this class
```c#
List<MapClassVariable> Variables { get; } 
```
List of properties exposed to tools for this class.
## Methods

```c#
override string ToString( ) 
```
OverridesObject.ToString
