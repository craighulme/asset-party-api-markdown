# PanelTreeNode

## Derives from TreeNode<IPanel>

## Summary

OverridesTreeNode.ValueHashIf the hash code changes we'll re-evaluate this node
## Constructors

```c#
PanelTreeNode( IPanel panel) 
```
No Summary
## Properties

```c#
override int ValueHash { get; } 
```
OverridesTreeNode.ValueHashIf the hash code changes we'll re-evaluate this node
## Methods

```c#
protected override void BuildChildren( ) 
```
OverridesTreeNode.BuildChildren
```c#
protected override bool HasDescendant( object obj) 
```
OverridesTreeNode.HasDescendantFill this out in your node to allow the tree system to work out
whether this object lies within your node's unexpanded children.
This should return true if the passed in object is a decendant of
this node - no matter how deep.
```c#
override bool OnContextMenu( ) 
```
OverridesTreeNode.OnContextMenuThe node has been right clicked. Return true to override default path
```c#
override void OnPaint( VirtualWidget item) 
```
OverridesTreeNode.OnPaint
