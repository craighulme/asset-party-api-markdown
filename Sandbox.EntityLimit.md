# EntityLimit

## Derives from object

## Summary

A class that limits the amount of entities.
## Constructors

```c#
EntityLimit( ) 
```
No Summary
## Properties

```c#
virtual int MaxTotal { get; set; } 
```
Maximum entities in this list before we start deleting
```c#
List<Entity> List { get; protected set; } 
```
List of entities currently in this shit
## Methods

```c#
void Retire( Entity ent) 
```
Delete this entity and remove it from the list
```c#
void Watch( ModelEntity ent) 
```
Watch an entity, contribute to the count and delete when its their turn
