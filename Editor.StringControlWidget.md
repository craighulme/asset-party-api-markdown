# StringControlWidget

## ```c#
Derives from ControlWidget
```

## Summary

OverridesControlWidget.IsControlActive
## Constructors

```c#
StringControlWidget( SerializedProperty property) 
```
No Summary
## Fields

```c#
protected LineEdit LineEdit
```
No Summary
## Properties

```c#
override bool IsControlActive { get; } 
```
OverridesControlWidget.IsControlActive
## Methods

```c#
protected virtual object StringToValue( string text) 
```
No Summary
```c#
protected virtual string ValueToString( ) 
```
No Summary
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
protected override void OnValueChanged( ) 
```
OverridesControlWidget.OnValueChanged
```c#
protected override Vector2 SizeHint( ) 
```
OverridesControlWidget.SizeHintShould return the size this widget really wants to be if it can its way. The default
is that you don't care - and just to return whatever the base value is.
## Inheriting Types

