# ChangeAttribute

## 
```c#
Derives from Attribute
```

## Summary

Combined with[Net]or[ConVar], this will invoke a method when the property changes.If no name is provided, we will try to call On[PropertyName]Changed.The callback should have 2 arguments - oldValue and newValue, both of the same type as the property itself.
## Remarks

## Constructors

```c#
ChangeAttribute( string name = null) 
```
No Summary
## Fields

```c#
string Name
```
Name of the method to call on change.
