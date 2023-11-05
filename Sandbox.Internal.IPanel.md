# IPanel

## Is interface
Inherits IValid

## Summary

Get all style blocks active on this panel
## Properties

```c#
abstract IEnumerable<IStyleBlock> ActiveStyleBlocks { get; } 
```
Get all style blocks active on this panel
```c#
abstract PanelInputType ButtonInput { get; set; } 
```
No Summary
```c#
abstract IEnumerable<IPanel> Children { get; } 
```
No Summary
```c#
abstract int ChildrenCount { get; } 
```
No Summary
```c#
abstract string Classes { get; } 
```
No Summary
```c#
abstract string ElementName { get; } 
```
No Summary
```c#
abstract Matrix? GlobalMatrix { get; } 
```
No Summary
```c#
abstract bool HasTooltip { get; } 
```
No Summary
```c#
abstract string Id { get; } 
```
The Id of the element ( id="foo" )
```c#
abstract Rect InnerRect { get; } 
```
No Summary
```c#
abstract bool IsCreatedByTemplate { get; } 
```
No Summary
```c#
abstract bool IsGame { get; } 
```
No Summary
```c#
abstract bool IsMainMenu { get; } 
```
No Summary
```c#
abstract bool IsVisible { get; } 
```
No Summary
```c#
abstract bool IsVisibleSelf { get; } 
```
No Summary
```c#
abstract Rect OuterRect { get; } 
```
No Summary
```c#
abstract IPanel Parent { get; } 
```
No Summary
```c#
abstract PseudoClass PseudoClass { get; set; } 
```
Procedural classes such as :hover and :active
```c#
abstract Rect Rect { get; } 
```
No Summary
```c#
abstract string SourceFile { get; } 
```
If the panel created by razor, this is the file in which it was defined
```c#
abstract int SourceLine { get; } 
```
If the panel was created by razor, this is the line in which it was defined
```c#
abstract bool WantsPointerEvents { get; } 
```
If true then this panel (or its ancestor) has pointer-events: all
## Methods

```c#
abstract IPanel CreateTooltip( ) 
```
No Summary
```c#
abstract void Delete( bool immediate) 
```
No Summary
```c#
abstract IPanel GetPanelAt( Vector2 point, bool visibleOnly, bool needPointerEvents = false) 
```
No Summary
```c#
abstract bool IsAncestor( IPanel panel) 
```
No Summary
```c#
abstract void SetAbsolutePosition( TextFlag alignment, Vector2 position, float offset) 
```
Set the panel's absolute position. This wouldn't be needed if we could expose the styles. Which we should
do.
```c#
abstract void UpdateTooltip( IPanel tooltipPanel) 
```
No Summary
