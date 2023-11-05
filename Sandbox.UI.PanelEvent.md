# PanelEvent

## 
```c#
Derives from object
```

## Summary

BaseUI.Panelevent.SeePanel.CreateEvent.
## Constructors

```c#
PanelEvent( string event_name, Panel active = null) 
```
No Summary
## Fields

```c#
string Button
```
No Summary
```c#
string Name
```
No Summary
```c#
Panel Target
```
No Summary
```c#
float Time
```
No Summary
```c#
object Value
```
No Summary
## Properties

```c#
Panel This { get; set; } 
```
The panel on which the event is being called.
For example, if you have a button with a label.. when the button gets clicked the actual click event
might come from the label. When the event is called on the label, This will be the label. When the event
propagates up to the button This will be the button - but Target will be the label. This is mainly of
use with Razor callbacks, where you want to get the actual panel that created the event.
## Methods

```c#
bool Is( string name) 
```
No Summary
```c#
void StopPropagation( ) 
```
No Summary
## Inheriting Types

