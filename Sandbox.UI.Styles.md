# Styles

## Derives from BaseStyles

## Summary

Represents all supported CSS properties and their currently assigned values.
## Constructors

```c#
Styles( ) 
```
No Summary
## Fields

```c#
static readonly Styles Default
```
No Summary
```c#
ShadowList BoxShadow
```
No Summary
```c#
ShadowList FilterDropShadow
```
No Summary
```c#
ShadowList TextShadow
```
No Summary
```c#
TransitionList Transitions
```
List of transitions this style sheet has.
## Properties

```c#
Color? BorderColor { set; } 
```
No Summary
```c#
Length? BorderWidth { set; } 
```
No Summary
```c#
bool HasTransitions { get; } 
```
Whether this style sheet has any transitions that would need to be run.
```c#
Length? Margin { set; } 
```
No Summary
```c#
Length? Padding { set; } 
```
No Summary
## Methods

```c#
bool ApplyAnimation( Panel panel) 
```
No Summary
```c#
Matrix BuildTransformMatrix( Vector2 size) 
```
Creates a matrix based on this style's "transform" and other related properties
```c#
Margin GetInset( Vector2 size) 
```
No Summary
```c#
Margin GetOutset( Vector2 size) 
```
No Summary
```c#
bool Set( string styles) 
```
No Summary
```c#
override void Add( BaseStyles bs) 
```
OverridesBaseStyles.AddCopy over only the styles that are set.
```c#
override void Dirty( ) 
```
OverridesBaseStyles.DirtyCalled when any CSS properties are changed.
```c#
override void From( BaseStyles bs) 
```
OverridesBaseStyles.FromCopy all styles from given style set.
```c#
override void FromLerp( BaseStyles from, BaseStyles to, float delta) 
```
OverridesBaseStyles.FromLerpLerp every property in this stylesheet
```c#
override void LerpProperty( string name, BaseStyles from, BaseStyles to, float delta) 
```
OverridesBaseStyles.LerpPropertyLerp a specific property by name
```c#
override bool Set( string property, string value) 
```
OverridesBaseStyles.SetCopy all styles from given style set.
## Nested Types

## Inheriting Types

