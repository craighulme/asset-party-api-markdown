# MapEntity

## 
```c#
Derives from MapNode
```

## Summary

MapEntity in Hammer is a type ofMapDoc.MapNodethat has a set of key/value pairs.
The keyvalues represent the authoritative state of the entity.Entities may have helpers that enhance the presentation and sometimes modification of those keyvalues.
The helpers may come and go; it should always be possible to recreate the helpers from
the parent entity's keyvalues.Entities may also have zero or moreMapDoc.MapMeshchildren.
## Constructors

```c#
MapEntity( MapDocument mapDocument = null) 
```
No Summary
## Properties

```c#
string ClassName { get; set; } 
```
Entity class name like prop_physics
```c#
MapClass MapClass { get; } 
```
No Summary
```c#
SerializedObject SerializedObject { get; } 
```
No Summary
```c#
TypeDescription TypeDescription { get; } 
```
No Summary
## Methods

```c#
string GetKeyValue( string key) 
```
Gets the value for the key, e.g "model" could return "models/props_c17/oildrum001_explosive.mdl"
```c#
void SetDefaultBounds( Vector3 min, Vector3 max) 
```
Sets the default bounds of the entity if it doesn't have a model. By default this is 16x16x16.
```c#
void SetKeyValue( string key, string value) 
```
Sets the value for the key, e.g "model" could be set to "models/props_c17/oildrum001_explosive.mdl"
