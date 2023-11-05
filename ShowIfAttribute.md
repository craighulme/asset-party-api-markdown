# ShowIfAttribute

## Derives from HideIfAttribute

## Summary

Show this property if a given property within the same class has the given value. Used typically in the Editor Inspector.
## Constructors

```c#
ShowIfAttribute( string propertyName, object value) 
```
No Summary
## Methods

```c#
override bool TestCondition( object targetObject, TypeDescription td) 
```
OverridesHideIfAttribute.TestConditionThe test condition.
