# MousePanelEvent

## ```c#
Derives from PanelEvent
```

## Summary

Mouse relatedUI.PanelEvent.
## Constructors

```c#
MousePanelEvent( string event_name, Panel active, string button) 
```
No Summary
## Fields

```c#
string Button
```
Which button triggered the event, in string form.
```c#
Vector2 LocalPosition
```
Position of the cursor relative to the panel's top left corner at the time the event was triggered.
## Properties

```c#
MouseButtons MouseButton { get; set; } 
```
Which button triggered the event, as aSandbox.MouseButtonsenum.
