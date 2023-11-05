# Section

## Derives from TreeNode

## Summary

OverridesTreeNode.ExpanderFillsIf a node returns true, you can expand by clicking anywhere on the node.
## Constructors

```c#
Section( string icon, string name, bool showCounts = false) 
```
No Summary
## Properties

```c#
string CountOverride { get; set; } 
```
No Summary
```c#
string Icon { get; set; } 
```
No Summary
```c#
Color IconColor { get; set; } 
```
No Summary
```c#
bool ShowCounts { get; set; } 
```
No Summary
```c#
string Title { get; set; } 
```
No Summary
```c#
override bool ExpanderFills { get; } 
```
OverridesTreeNode.ExpanderFillsIf a node returns true, you can expand by clicking anywhere on the node.
```c#
override bool ExpanderHidden { get; } 
```
OverridesTreeNode.ExpanderHiddenIf true the default expander won't be drawn
## Methods

```c#
override void OnPaint( VirtualWidget item) 
```
OverridesTreeNode.OnPaint
