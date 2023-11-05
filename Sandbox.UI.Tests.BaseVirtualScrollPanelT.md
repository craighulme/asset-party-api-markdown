# BaseVirtualScrollPanel<T>

## Is abstract
Derives from Panel

## Summary

Return true if we have this data slot
## Type Parameters

```c#
T is class, 
```
No Summary
## Constructors

```c#
BaseVirtualScrollPanel( ) 
```
No Summary
## Fields

```c#
Dictionary<int, Panel> CreatedPanels
```
No Summary
```c#
GridLayout Layout
```
No Summary
## Properties

```c#
bool NeedsRebuild { get; set; } 
```
No Summary
## Methods

```c#
abstract T GetItem( int i) 
```
No Summary
```c#
abstract bool HasData( int i) 
```
Return true if we have this data slot
```c#
abstract int ItemCount( ) 
```
No Summary
```c#
abstract void OnCellCreated( int index, T item, Panel cell) 
```
No Summary
```c#
void RefreshCreated( int i) 
```
No Summary
```c#
protected override void FinalLayoutChildren( Vector2 offset) 
```
OverridesPanel.FinalLayoutChildrenLayout the children of this panel.
```c#
override void SetProperty( string name, string value) 
```
OverridesPanel.SetPropertySet a property on the panel, such as special properties (class,id,styleandvalue, etc.) and properties of the panel's C# class.
```c#
override void Tick( ) 
```
OverridesPanel.TickCalled every frame. This is your "Think" function.
