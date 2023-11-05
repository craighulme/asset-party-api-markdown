# BaseInventory

## 
```c#
Implements IBaseInventory
```

## Summary

ImplementsIBaseInventory.Active
## Constructors

```c#
BaseInventory( Entity owner) 
```
No Summary
## Fields

```c#
List<Entity> List
```
No Summary
## Properties

```c#
virtual Entity Active { get; set; } 
```
ImplementsIBaseInventory.Active
```c#
Entity Owner { get; init; } 
```
No Summary
## Methods

```c#
virtual bool Add( Entity ent, bool makeActive = false) 
```
ImplementsIBaseInventory.AddTry to add this entity to the inventory. Will return true
if the entity was added successfully.
```c#
virtual bool CanAdd( Entity ent) 
```
Return true if this item belongs in the inventory
```c#
virtual bool Contains( Entity ent) 
```
ImplementsIBaseInventory.ContainsReturns true if this inventory contains this entity
```c#
virtual int Count( ) 
```
ImplementsIBaseInventory.CountReturns the number of items in the inventory
```c#
virtual void DeleteContents( ) 
```
ImplementsIBaseInventory.DeleteContentsDelete every entity we're carrying. Useful to call on death.
```c#
virtual bool Drop( Entity ent) 
```
ImplementsIBaseInventory.DropDrop this entity. Will return true if successfully dropped.
```c#
virtual Entity DropActive( ) 
```
ImplementsIBaseInventory.DropActiveDrop the active entity. If we can't drop it, will return null
```c#
virtual int GetActiveSlot( ) 
```
ImplementsIBaseInventory.GetActiveSlotReturns the index of the currently active child
```c#
virtual Entity GetSlot( int i) 
```
ImplementsIBaseInventory.GetSlotGet the item in this slot
```c#
virtual void OnChildAdded( Entity child) 
```
ImplementsIBaseInventory.OnChildAddedA child has been added to the Owner (player). Do we want this
entity in our inventory? Yeah? Add it then.
```c#
virtual void OnChildRemoved( Entity child) 
```
ImplementsIBaseInventory.OnChildRemovedA child has been removed from our Owner. This might not even
be in our inventory, if it is then we'll remove it from our list
```c#
virtual void Pickup( Entity ent) 
```
Try to pick this entity up
```c#
virtual bool SetActive( Entity ent) 
```
ImplementsIBaseInventory.SetActiveMake this entity the active one
```c#
virtual bool SetActiveSlot( int i, bool evenIfEmpty = false) 
```
ImplementsIBaseInventory.SetActiveSlotSet our active entity to the entity on this slot
```c#
virtual bool SwitchActiveSlot( int idelta, bool loop) 
```
ImplementsIBaseInventory.SwitchActiveSlotSwitch to the slot next to the slot we have active.
