# NoticeManager

## Is static
Derives from object

## Summary

Manages those annoying notices on the side of your screen. You get them when you're compiling.
This is what's making those errors keep appearing. It's not your bad code, it's this bad class,
blame this class - it's this classes fault you're getting annoyed.
## Properties

```c#
static IEnumerable<Widget> All { get; } 
```
No Summary
## Methods

```c#
static void Add( Widget widget) 
```
Add a new widget. Derive your widget from NoticeWidget to win big prizes!
```c#
static void ClearAll( ) 
```
Instantly destroy all notifications
```c#
static void Dismiss( Widget widget) 
```
We're done with this widget, get rid of it straight away, even if we're hovering over it.
```c#
static void Remove( Widget widget, float timeDelay = 2) 
```
Remove this widget in timeDelay seconds. If we're already removing it, this will only have
an effect is timeDelay is lower than the current delay until we're being removed
```c#
static void Tick( ) 
```
No Summary
