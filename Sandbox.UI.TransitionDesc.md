# TransitionDesc

## 
```c#
Derives from ValueType
```

## Summary

Describes transition of a single CSS property, a.k.a. the values of atransitionCSS property.Utility to create a transition by comparing the
panel style before and after the scope.
## Fields

```c#
float? Delay
```
If set, delay before starting the transition after the property was changed.
```c#
float? Duration
```
Duration of the transition between old value and new value.
```c#
string Property
```
The CSS property to transition.
```c#
string TimingFunction
```
The timing or "easing" function.transition-timing-functionCSS property.
Example values would beease,ease-in,ease-outandease-in-out.
## Referencing Members

```c#
List<TransitionDesc> = TransitionList.List
```
