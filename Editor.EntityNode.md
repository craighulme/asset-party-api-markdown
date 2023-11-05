# EntityNode

## ```c#
Derives from TreeNode<EntityEntry>
```

## Summary

OverridesTreeNode.ValueHashIf the hash code changes we'll re-evaluate this node
## Constructors

```c#
EntityNode( EntityEntry obj) 
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
override bool OnContextMenu( ) 
```
OverridesTreeNode.OnContextMenuThe node has been right clicked. Return true to override default path
```c#
override void OnPaint( VirtualWidget item) 
```
OverridesTreeNode.OnPaint
```c#
override void OnSelectionChanged( bool state) 
```
OverridesTreeNode.OnSelectionChanged
