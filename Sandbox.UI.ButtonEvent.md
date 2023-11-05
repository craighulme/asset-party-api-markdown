# ButtonEvent

## Derives from object
Implements IEquatable< ButtonEvent>

## Summary

Keyboard (and mouse) key pressUI.PanelEvent.
## Constructors

```c#
protected ButtonEvent( ButtonEvent original) 
```
No Summary
## Properties

```c#
string Button { get; } 
```
The button that triggered the event.
```c#
bool HasAlt { get; } 
```
WhetherAltkey was being held down at the time of the event.
```c#
bool HasCtrl { get; } 
```
WhetherControlkey was being held down at the time of the event.
```c#
bool HasShift { get; } 
```
WhetherShiftkey was being held down at the time of the event.
```c#
KeyboardModifiers KeyboardModifiers { get; } 
```
The keyboard modifier keys that were held down at the moment the event triggered.
```c#
bool Pressed { get; } 
```
Whether the button was pressed in, or release.
```c#
bool StopPropagation { get; set; } 
```
Set totrueto prevent the event from propagating to the parent panel.
```c#
int VirtualKey { get; } 
```
No Summary
## Methods

```c#
override bool Equals( object obj) 
```
OverridesObject.Equals
```c#
override bool Equals( ButtonEvent other) 
```
OverridesObject.Equals
```c#
override int GetHashCode( ) 
```
OverridesObject.GetHashCode
```c#
override string ToString( ) 
```
OverridesObject.ToString
## Operators

```c#
bool ==( ButtonEvent left, ButtonEvent right) 
```
No Summary
```c#
bool !=( ButtonEvent left, ButtonEvent right) 
```
No Summary
