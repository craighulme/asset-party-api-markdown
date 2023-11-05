# StyleSelector

## 
```c#
Derives from object
```

## Summary

A CSS selector like "Panel.button.red:hover .text"
## Constructors

```c#
StyleSelector( ) 
```
No Summary
## Fields

```c#
StyleSelector[] AnyOf
```
No Summary
```c#
string AsString
```
No Summary
```c#
StyleBlock Block
```
No Summary
```c#
StyleSelector[] DecendantOf
```
No Summary
```c#
string Element
```
No Summary
```c#
PseudoClass Flags
```
No Summary
```c#
bool ImmediateParent
```
No Summary
```c#
StyleSelector Not
```
No Summary
```c#
Func<Panel, bool> NthChild
```
No Summary
```c#
StyleSelector Parent
```
Descendant combinator
A B
Child combinator
A > B
Adjacent sibling combinator
A + B
General sibling combinator
A ~B
```c#
int SelfScore
```
No Summary
```c#
bool UniversalSelector
```
True if this has a universal selector (*)
## Properties

```c#
string Id { get; set; } 
```
The Id selector - minus the #https://developer.mozilla.org/en-US/docs/Web/CSS/ID_selectors
```c#
int Score { get; } 
```
No Summary
## Methods

```c#
bool Test( Panel panel) 
```
No Summary
```c#
bool TestBroadphase( Panel panel) 
```
No Summary
```c#
bool TestParent( Panel panel, bool recusive = true) 
```
No Summary
