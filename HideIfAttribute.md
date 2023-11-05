# HideIfAttribute

## Derives from ConditionalVisibilityAttribute

## Summary

Hide this property if a given property within the same class has the given value. Used typically in the Editor Inspector.
## Constructors

```c#
HideIfAttribute( string propertyName, object value) 
```
No Summary
## Properties

```c#
string PropertyName { get; set; } 
```
Property name to test.
```c#
object Value { get; set; } 
```
Property value to test against.
## Methods

```c#
override bool TestCondition( object targetObject, TypeDescription td) 
```
OverridesConditionalVisibilityAttribute.TestConditionThe test condition.
## Inheriting Types

