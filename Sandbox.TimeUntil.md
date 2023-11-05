# TimeUntil

## 
```c#
Implements IEquatable<TimeUntil>
```

## Summary

A convenience struct to easily manage a time countdown, based onTime.Now.Typical usage would see you assigning to a variable of this type a necessary amount of seconds.
Then the struct would return the time countdown, or can be used as a bool i.e.:TimeUntil nextAttack = 10;
if ( nextAttack ) { /*Do something*/ }
## Properties

```c#
float Absolute { get; } 
```
Time to which we are counting down to, based onTime.Now.
```c#
float Fraction { get; } 
```
The countdown, but as a fraction, i.e. a value from 0 (start of countdown) to 1 (end of countdown)
```c#
float Passed { get; } 
```
Amount of seconds passed since the countdown started.
```c#
float Relative { get; } 
```
The actual countdown, in seconds.
## Methods

```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( TimeUntil o) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
```c#
override string ToString( ) 
```
OverridesValueType.ToString
## Operators

```c#
bool ==( TimeUntil left, TimeUntil right) 
```
No Summary
```c#
bool >( in TimeUntil ts, float f) 
```
No Summary
```c#
bool >( in TimeUntil ts, int f) 
```
No Summary
```c#
bool >=( in TimeUntil ts, float f) 
```
No Summary
```c#
bool >=( in TimeUntil ts, int f) 
```
No Summary
```c#
bool !=( TimeUntil left, TimeUntil right) 
```
No Summary
```c#
bool <( in TimeUntil ts, float f) 
```
No Summary
```c#
bool <( in TimeUntil ts, int f) 
```
No Summary
```c#
bool <=( in TimeUntil ts, float f) 
```
No Summary
```c#
bool <=( in TimeUntil ts, int f) 
```
No Summary
```c#
implicit bool =( TimeUntil ts) 
```
No Summary
```c#
implicit float =( TimeUntil ts) 
```
No Summary
```c#
implicit TimeUntil =( float ts) 
```
No Summary
