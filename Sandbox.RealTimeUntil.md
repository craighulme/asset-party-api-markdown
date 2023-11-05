# RealTimeUntil

## Derives from ValueType
Implements IEquatable< RealTimeUntil>

## Summary

A convenience struct to easily manage a time countdown, based onRealTime.GlobalNow.Typical usage would see you assigning to a variable of this type a necessary amount of seconds.
Then the struct would return the time countdown, or can be used as a bool i.e.:RealTimeUntil nextAttack = 10;
if ( nextAttack ) { /*Do something*/ }
## Properties

```c#
double Absolute { get; } 
```
Time to which we are counting down to, based onRealTime.GlobalNow.
```c#
double Fraction { get; } 
```
The countdown, but as a fraction, i.e. a value from 0 (start of countdown) to 1 (end of countdown)
```c#
double Passed { get; } 
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
override bool Equals( RealTimeUntil o) 
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
bool ==( RealTimeUntil left, RealTimeUntil right) 
```
No Summary
```c#
bool >( in RealTimeUntil ts, float f) 
```
No Summary
```c#
bool >( in RealTimeUntil ts, int f) 
```
No Summary
```c#
bool >=( in RealTimeUntil ts, float f) 
```
No Summary
```c#
bool >=( in RealTimeUntil ts, int f) 
```
No Summary
```c#
bool !=( RealTimeUntil left, RealTimeUntil right) 
```
No Summary
```c#
bool <( in RealTimeUntil ts, float f) 
```
No Summary
```c#
bool <( in RealTimeUntil ts, int f) 
```
No Summary
```c#
bool <=( in RealTimeUntil ts, float f) 
```
No Summary
```c#
bool <=( in RealTimeUntil ts, int f) 
```
No Summary
```c#
implicit bool =( RealTimeUntil ts) 
```
No Summary
```c#
implicit float =( RealTimeUntil ts) 
```
No Summary
```c#
implicit RealTimeUntil =( float ts) 
```
No Summary
## Referencing Members

```c#
RealTimeUntil = Prop.Invulnerable { get; set; } 
```
