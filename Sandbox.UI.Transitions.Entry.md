# Entry

## Derives from ValueType

## Summary

OverridesValueType.ToString
## Constructors

```c#
Entry( string property, float startTime, float length, int target, TransitionFunction action, Function easingFunction) 
```
No Summary
## Properties

```c#
TransitionFunction Action { get; init; } 
```
No Summary
```c#
Function EasingFunction { get; init; } 
```
No Summary
```c#
bool IsKilled { get; } 
```
No Summary
```c#
float Length { get; init; } 
```
No Summary
```c#
string Property { get; init; } 
```
No Summary
```c#
float StartTime { get; init; } 
```
No Summary
```c#
int Target { get; init; } 
```
No Summary
## Methods

```c#
float Ease( float delta) 
```
No Summary
```c#
void Invoke( Styles style, float delta) 
```
No Summary
```c#
override string ToString( ) 
```
OverridesValueType.ToString
## Referencing Members

```c#
List<Entry> = Transitions.Entries
```
