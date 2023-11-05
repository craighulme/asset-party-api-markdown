# EventAttribute

## 
```c#
Derives from Attribute
```

## Summary

A generic event listener. You are probably looking for Sandbox.Event.* attributes.
## Constructors

```c#
EventAttribute( string eventName) 
```
No Summary
## Properties

```c#
string EventName { get; set; } 
```
The internal event identifier.
```c#
int Priority { get; set; } 
```
Events with lower numbers are run first. This defaults to 0, so setting it to -1 will mean your
event will run before all other events that don't define it. Setting it to 1 would mean it'll
run after all events that don't.
## Inheriting Types

