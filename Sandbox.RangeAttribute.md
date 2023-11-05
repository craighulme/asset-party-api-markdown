# RangeAttribute

## Derives from Attribute

## Summary

Mark this property as a ranged float/int. In inspector we'll be able to create a slider
instead of a text entry.
TODO: Replace this with the System.ComponentModel.DataAnnotations.Range one - move step and clamped to their own attributes
## Constructors

```c#
RangeAttribute( float min, float max, float step = 0.01, bool clamped = true) 
```
No Summary
## Properties

```c#
bool Clamped { get; } 
```
No Summary
```c#
float Max { get; } 
```
No Summary
```c#
float Min { get; } 
```
No Summary
```c#
float Step { get; } 
```
No Summary
## Inheriting Types

