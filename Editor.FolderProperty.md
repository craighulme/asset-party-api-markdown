# FolderProperty

## ```c#
Derives from LineEdit
```

## Summary

An editable text box with a button to browse for an arbitrary folder using OS file browser dialog.
## Constructors

```c#
FolderProperty( Widget parent) 
```
No Summary
## Fields

```c#
Action<string> FolderSelected
```
Path to the user selected folder.
## Properties

```c#
string DialogTitle { get; set; } 
```
Title override for the "browse folder" dialog.
## Methods

```c#
void Browse( ) 
```
Open a "browse folder" dialog.
```c#
override void OnDragDrop( DragEvent ev) 
```
OverridesWidget.OnDragDropSomething was dragged and dropped on this widget. Apply the data here, if its valid.RequiresWidget.AcceptDropsto function.
```c#
override void OnDragHover( DragEvent ev) 
```
OverridesWidget.OnDragHoverCursor with drag and drop data moved on this widget.RequiresWidget.AcceptDropsto function.
```c#
protected override void OnMouseEnter( ) 
```
OverridesWidget.OnMouseEnterMouse cursor entered the bounds of this widget.
```c#
protected override void OnMouseLeave( ) 
```
OverridesWidget.OnMouseLeaveMouse cursor exited the bounds of this widget.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
