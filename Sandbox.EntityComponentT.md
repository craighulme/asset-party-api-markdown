# EntityComponent<T>

## 
```c#
Derives from EntityComponent
```

## Summary

Component that can be only added to given entity type.
## Type Parameters

```c#
T is Entity, 
```
No Summary
## Constructors

```c#
EntityComponent( ) 
```
No Summary
## Properties

```c#
T Entity { get; } 
```
ImplementsEntityComponent.EntityThe entity this component is attached to.
## Methods

```c#
override bool CanAddToEntity( Entity entity) 
```
OverridesEntityComponent.CanAddToEntityReturn false if target entity is not of type T
