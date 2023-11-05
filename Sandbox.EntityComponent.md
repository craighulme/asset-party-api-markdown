# EntityComponent

## Derives from BaseNetworkable
Implements IComponent

## Summary

Generic entity component.
## Constructors

```c#
EntityComponent( ) 
```
No Summary
## Properties

```c#
virtual bool Enabled { get; set; } 
```
ImplementsIComponent.EnabledWhether this component is enabled or not.
```c#
virtual bool IsClientOnly { get; } 
```
ImplementsIComponent.IsClientOnlyTrue if this component only exists on the client
```c#
virtual bool IsServerOnly { get; } 
```
ImplementsIComponent.IsServerOnlyTrue if this component only exists on the server
```c#
virtual string Name { get; set; } 
```
ImplementsIComponent.NameName of the component, will be shown in entity inspector
```c#
Entity Entity { get; } 
```
The entity this component is attached to.
```c#
Prefab Prefab { get; set; } 
```
If created via a prefab, this will be the prefab it was created from
```c#
int PrefabGuid { get; set; } 
```
If created via a prefab, this will be the guid of the matching component inside
```c#
bool ShouldTransmit { get; protected set; } 
```
Whether this component should transmit to client or not.
```c#
override int NetworkIdent { get; } 
```
OverridesBaseNetworkable.NetworkIdentShould return an ID of this networkable that is common across the network
## Methods

```c#
static IEnumerable<T> GetAllOfType<T,>( ) 
```
Returns all active (Enabled) components of given type.
```c#
virtual bool CanAddToEntity( Entity entity) 
```
Return false if can't be added to this entity for some reason
```c#
protected virtual void OnActivate( ) 
```
Called when this component is enabled (or added to the entity)
```c#
protected virtual void OnDeactivate( ) 
```
Called when this component is disabled (or removed from the entity)
```c#
void Remove( ) 
```
Remove this component from the parent entity. Entity will become null immediately,
so don't try to access it after calling this!
```c#
override string ToString( ) 
```
OverridesObject.ToString
## Inheriting Types

