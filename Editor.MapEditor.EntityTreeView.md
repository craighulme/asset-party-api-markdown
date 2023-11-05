# EntityTreeView

## ```c#
Derives from TreeView
```

## Summary

OverridesTreeView.SetSelectedSet the selected object state. If state is true and ExpandForSelection is true, we'll
try to expand the tree path to the selected object.
## Constructors

```c#
EntityTreeView( Widget parent) 
```
No Summary
## Properties

```c#
Action<string> OnItemSelected { get; set; } 
```
No Summary
## Methods

```c#
override void SetSelected( object obj, bool state, bool skipEvents) 
```
OverridesTreeView.SetSelectedSet the selected object state. If state is true and ExpandForSelection is true, we'll
try to expand the tree path to the selected object.
