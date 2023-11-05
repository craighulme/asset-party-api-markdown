# Header

## 
```c#
Derives from TreeNode
```

## Summary

OverridesTreeNode.ExpanderFillsIf a node returns true, you can expand by clicking anywhere on the node.
## Constructors

```c#
Header( string icon, string name, bool showCounts = false) 
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
## Methods

```c#
override void OnPaint( VirtualWidget item) 
```
OverridesTreeNode.OnPaint
