# TreeNode

## 
```c#
Derives from object
```

## Summary

If a node returns true, you can expand by clicking anywhere on the node.
## Constructors

```c#
TreeNode( object value) 
```
No Summary
```c#
TreeNode( ) 
```
No Summary
## Properties

```c#
virtual bool ExpanderFills { get; } 
```
If a node returns true, you can expand by clicking anywhere on the node.
```c#
virtual bool ExpanderHidden { get; } 
```
If true the default expander won't be drawn
```c#
virtual bool HasChildren { get; } 
```
No Summary
```c#
virtual int ValueHash { get; } 
```
If the hash code changes we'll re-evaluate this node
```c#
IEnumerable<TreeNode> Children { get; } 
```
No Summary
```c#
float Height { get; set; } 
```
No Summary
```c#
TreeNode Parent { get; } 
```
No Summary
```c#
TreeView TreeView { get; } 
```
No Summary
```c#
object Value { get; set; } 
```
No Summary
## Methods

```c#
protected virtual void BuildChildren( ) 
```
No Summary
```c#
virtual void Clear( ) 
```
No Summary
```c#
virtual string GetTooltip( ) 
```
No Summary
```c#
virtual bool HasAncestor( object obj) 
```
Return true if this value or tree node is one of our ancestors
```c#
protected virtual bool HasDescendant( object obj) 
```
Fill this out in your node to allow the tree system to work out
whether this object lies within your node's unexpanded children.
This should return true if the passed in object is a decendant of
this node - no matter how deep.
```c#
virtual void OnActivated( ) 
```
Called when the item is double clicked, or selected and enter is pressed
```c#
virtual bool OnContextMenu( ) 
```
The node has been right clicked. Return true to override default path
```c#
virtual DropAction OnDragDrop( ItemDragEvent e) 
```
No Summary
```c#
virtual void OnDragHover( DragEvent ev) 
```
No Summary
```c#
virtual bool OnDragStart( ) 
```
No Summary
```c#
virtual void OnDrop( DragEvent ev) 
```
No Summary
```c#
protected virtual void OnHashChanged( ) 
```
The value of ValueHash has changed
```c#
virtual void OnKeyPress( KeyEvent e) 
```
No Summary
```c#
virtual void OnPaint( VirtualWidget item) 
```
No Summary
```c#
virtual void OnSelectionChanged( bool state) 
```
No Summary
```c#
protected virtual void RebuildOnDirty( ) 
```
No Summary
```c#
virtual TreeNode ResolveNode( object obj, bool createPath) 
```
No Summary
```c#
protected virtual void Think( ) 
```
No Summary
```c#
void AddItem( object item) 
```
No Summary
```c#
void AddItems( IEnumerable<object> items) 
```
No Summary
```c#
void Dirty( ) 
```
No Summary
```c#
IEnumerable<TreeNode> EnumeratePathTo( TreeNode node) 
```
No Summary
```c#
void OnVisible( ) 
```
No Summary
```c#
protected void PaintSelection( VirtualWidget item) 
```
Paint the standard selection/hover/press highlight background
```c#
void RemoveItem( TreeNode item) 
```
No Summary
```c#
void SetChildren<T,>( IEnumerable<T> list, Func<T, TreeNode> createNode) 
```
Set the children to match this list.
Remove any that aren't in the list.
Use the function to create the node.
Make sure the order matches the incoming list.
```c#
void SetItems( IEnumerable<TreeNode> items) 
```
No Summary
```c#
override string ToString( ) 
```
OverridesObject.ToString
## Nested Types

## Inheriting Types

