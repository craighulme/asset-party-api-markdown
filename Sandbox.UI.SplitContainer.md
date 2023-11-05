# SplitContainer

## 
```c#
Derives from Panel
```

## Summary

A control that has two panes with a splitter in between. You can drag the splitter to change the size of the two panels.
## Constructors

```c#
SplitContainer( ) 
```
No Summary
## Fields

```c#
float MinimumFractionLeft
```
The smallest the left section can be as a fraction (0-1). Also controls the largest the right section can be.
```c#
float MinimumFractionRight
```
The smallest the right section can be as a fraction (0-1). Also controls the largest the left section can be.
## Properties

```c#
string FractionCookie { get; set; } 
```
We can save the position of this splitter in a cookie. To do that set this
(or "cookie" in a template). We'll automatically save and restore from the cookie.
```c#
bool IsDragging { get; protected set; } 
```
Returns true if splitter is being dragged
```c#
Panel Left { get; protected set; } 
```
The left, or top panel. Has class "split-left".
```c#
Panel Right { get; protected set; } 
```
The left, or bottom panel. Has class "split-right".
```c#
Panel Splitter { get; protected set; } 
```
The splitter control
```c#
bool Vertical { get; set; } 
```
Should this be laid out vertically? If you set this to vertical you should
mentally change Left to Top and Right to Bottom.
## Methods

```c#
virtual void UpdateSplitFraction( float f) 
```
Sets the split fraction to this value. Will automatically adjust the value
according to MinimumFraction parameters, and will save the new value to cookie.
```c#
protected override void OnMouseMove( MousePanelEvent e) 
```
OverridesPanel.OnMouseMoveIf we're dragging then position the split where the mouse is.
```c#
override void OnTemplateSlot( INode element, string slotName, Panel panel) 
```
OverridesPanel.OnTemplateSlotYou can create child panels in the template by setting attributes
on them, like slot="left" to make that panel appear in the left panel.
```c#
override void SetProperty( string name, string value) 
```
OverridesPanel.SetPropertySet a property on the panel, such as special properties (class,id,styleandvalue, etc.) and properties of the panel's C# class.
