# VirtualScrollPanel

## 
```c#
Derives from Panel
```

## Summary

Scroll panel that creates its contents as they become visibleTODO: we need to let panels know, or recreate them, when Data changes
## Constructors

```c#
VirtualScrollPanel( ) 
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
virtual List<object> Data { get; set; } 
```
No Summary
```c#
bool NeedsRebuild { get; set; } 
```
No Summary
```c#
Action<Panel, object> OnCreateCell { get; set; } 
```
Create a new panel. You should add a child to the passed panel (which is the cell).
## Methods

```c#
virtual void AddItem( object item) 
```
No Summary
```c#
virtual void Clear( ) 
```
No Summary
```c#
virtual void OnCellCreated( int i, Panel cell) 
```
No Summary
```c#
void AddItems( object[] items) 
```
No Summary
```c#
bool HasData( int i) 
```
Return true if we have this data slot
```c#
void RefreshCreated( int i) 
```
No Summary
```c#
void SetItems( IEnumerable<object> enumerable) 
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
