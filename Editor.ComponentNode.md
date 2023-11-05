# ComponentNode

## ```c#
Derives from TreeNode<IComponent>
```

## Summary

OverridesTreeNode.ValueHashIf the hash code changes we'll re-evaluate this node
## Constructors

```c#
ComponentNode( IComponent obj) 
```
No Summary
## Properties

```c#
override int ValueHash { get; } 
```
OverridesTreeNode.ValueHashIf the hash code changes we'll re-evaluate this node
## Methods

```c#
override void OnPaint( VirtualWidget item) 
```
OverridesTreeNode.OnPaint
```c#
override void OnSelectionChanged( bool state) 
```
OverridesTreeNode.OnSelectionChanged
