# EntityTarget

## 
```c#
Implements INetworkSerializer
```

## Summary

Describes a target for the Entity IO system. The description finds by name, or class name.
You can manually enumerate valid entities using EnumerateTargets
## Properties

```c#
string Name { get; set; } 
```
The target name or class name of entities to look for.
## Methods

```c#
static EntityTarget Default( string entity_or_class_name) 
```
Target an entity with a name or class name
```c#
static EntityTarget WithEntityName( string entityname) 
```
Target an entity with a specific name
```c#
virtual void Read( ref NetRead read) 
```
ImplementsINetworkSerializer.ReadRead an instance of this class from aSandbox.NetReader.
```c#
virtual void Write( NetWrite write) 
```
ImplementsINetworkSerializer.WriteWrite an instance of this class to aSandbox.NetWriter.
```c#
Entity GetTarget( Entity source_entity, Entity activator_entity) 
```
Returns the first entity that is a valid target.
```c#
T GetTarget<T,>( Entity source_entity, Entity activator_entity) 
```
Returns the first entity that is a valid target as is of given type.
```c#
Entity GetTarget( Entity source_entity = null) 
```
Returns the first entity that is a valid target.
```c#
T GetTarget<T,>( Entity source_entity = null) 
```
Returns the first entity that is a valid target as is of given type.
```c#
Entity[] GetTargets( Entity source_entity, Entity activator_entity) 
```
Get a list of entities that are appropriate targets for this
```c#
Entity[] GetTargets( Entity source_entity = null) 
```
Get a list of entities that are appropriate targets for this
```c#
bool IsValid( Entity source_entity, Entity activator_entity) 
```
Returns true if this class refers to at least one valid entity
```c#
bool IsValid( ) 
```
Returns true if this class refers to at least one valid entity
```c#
bool TestEntity( Entity ent) 
```
Check whether entity passes this target's test
```c#
bool TryGetTarget<T,>( out T target, Entity source_entity, Entity activator_entity) 
```
Try to get a target entity with given type.
```c#
bool TryGetTarget<T,>( out T target, Entity source_entity = null) 
```
Try to get a target entity with given type.
```c#
bool TryGetTargets<T,>( out T[] targets, Entity source_entity, Entity activator_entity) 
```
Try to get a list of entities that are appropriate targets for this.
```c#
bool TryGetTargets<T,>( out T[] targets, Entity source_entity = null) 
```
Try to get a list of entities that are appropriate targets for this.
```c#
override string ToString( ) 
```
OverridesValueType.ToString
## Operators

```c#
implicit EntityTarget =( string entity_or_class_name) 
```
No Summary
## Referencing Members

```c#
virtual void Entity.AddConnection( string, EntityTarget, string, string, float, int ) 
```
```c#
EntityTarget = MovementPathNodeEntity.AlternativeNodeBackwards { get; set; } 
```
```c#
EntityTarget = MovementPathNodeEntity.AlternativeNodeForwards { get; set; } 
```
```c#
EntityTarget = MonitorEntity.CameraName { get; set; } 
```
```c#
EntityTarget = ParticleSystemEntity.ControlPoint0 { get; set; } 
```
```c#
EntityTarget = ParticleSystemEntity.ControlPoint1 { get; set; } 
```
```c#
EntityTarget = ParticleSystemEntity.ControlPoint2 { get; set; } 
```
```c#
EntityTarget = ParticleSystemEntity.ControlPoint3 { get; set; } 
```
```c#
EntityTarget = ParticleSystemEntity.ControlPoint4 { get; set; } 
```
```c#
EntityTarget = ParticleSystemEntity.ControlPoint5 { get; set; } 
```
```c#
EntityTarget = BaseConstraint.EntityName1 { get; set; } 
```
```c#
EntityTarget = BaseConstraint.EntityName2 { get; set; } 
```
```c#
EntityTarget = DoorEntity.OtherDoorsToOpen { get; set; } 
```
```c#
EntityTarget = PathPlatformEntity.PathEntity { get; set; } 
```
```c#
EntityTarget = TeleportVolumeEntity.TargetEntity { get; set; } 
```
