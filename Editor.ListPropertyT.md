# ListProperty<T>

## ```c#
Derives from PropertyEditorWidget
```

## Summary

OverridesWidget.OnDragDropSomething was dragged and dropped on this widget. Apply the data here, if its valid.RequiresWidget.AcceptDropsto function.
## Type Parameters

```c#
T
```
No Summary
## Constructors

```c#
ListProperty( Widget parent) 
```
No Summary
## Properties

```c#
IList<T> Value { get; set; } 
```
No Summary
## Methods

```c#
void Rebuild( ) 
```
No Summary
```c#
override void OnDragDrop( DragEvent ev) 
```
OverridesWidget.OnDragDropSomething was dragged and dropped on this widget. Apply the data here, if its valid.RequiresWidget.AcceptDropsto function.
```c#
override void OnDragHover( DragEvent ev) 
```
OverridesWidget.OnDragHoverCursor with drag and drop data moved on this widget.RequiresWidget.AcceptDropsto function.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
