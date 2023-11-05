# RangedFloatSliderProperty

## Derives from Widget
Implements IEditorAttribute<MinMaxAttribute>, IEditorAttribute<RangeAttribute>

## Summary

ImplementsIEditorAttribute<T>.SetEditorAttribute
## Constructors

```c#
RangedFloatSliderProperty( Widget parent) 
```
No Summary
## Properties

```c#
RangeType RangeType { get; set; } 
```
No Summary
```c#
RangedFloat Value { get; set; } 
```
No Summary
## Methods

```c#
virtual void SetEditorAttribute( MinMaxAttribute attribute) 
```
ImplementsIEditorAttribute<T>.SetEditorAttribute
```c#
virtual void SetEditorAttribute( RangeAttribute attribute) 
```
ImplementsIEditorAttribute<T>.SetEditorAttribute
```c#
void RangeTypeChanged( ) 
```
No Summary
```c#
override void ChildValuesChanged( Widget source) 
```
OverridesWidget.ChildValuesChanged
