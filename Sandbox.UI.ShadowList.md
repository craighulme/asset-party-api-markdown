# ShadowList

## Derives from List< Shadow>

## Summary

A list of shadows
## Constructors

```c#
ShadowList( ) 
```
No Summary
## Fields

```c#
bool IsNone
```
Whether there are no shadows at all.
## Methods

```c#
void AddFrom( ShadowList other) 
```
Copy shadows from another list of shadows.
```c#
void SetFromLerp( ShadowList a, ShadowList b, float frac) 
```
Given 2 lists of shadows, perform linear interpolation on both lists and store the result in this list.
Will work with mismatched shadow counts.
```c#
override int GetHashCode( ) 
```
OverridesObject.GetHashCode
