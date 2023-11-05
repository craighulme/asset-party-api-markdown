# TimeSince

## Derives from ValueType
Implements IEquatable< TimeSince>

## Summary

A convenience struct to easily measure time since an event last happened, based onTime.Now.Typical usage would see you assigning 0 to a variable of this type to reset the timer.
Then the struct would return time since the last reset. i.e.:TimeSince lastUsed = 0;
if ( lastUsed > 10 ) { /*Do something*/ }
## Properties

```c#
float Absolute { get; } 
```
Time at which the timer reset happened, based onTime.Now.
```c#
float Relative { get; } 
```
Time passed since last reset, in seconds.
## Methods

```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( TimeSince o) 
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
bool ==( TimeSince left, TimeSince right) 
```
No Summary
```c#
bool >( in TimeSince ts, float f) 
```
No Summary
```c#
bool >( in TimeSince ts, int f) 
```
No Summary
```c#
bool >=( in TimeSince ts, float f) 
```
No Summary
```c#
bool >=( in TimeSince ts, int f) 
```
No Summary
```c#
bool !=( TimeSince left, TimeSince right) 
```
No Summary
```c#
bool <( in TimeSince ts, float f) 
```
No Summary
```c#
bool <( in TimeSince ts, int f) 
```
No Summary
```c#
bool <=( in TimeSince ts, float f) 
```
No Summary
```c#
bool <=( in TimeSince ts, int f) 
```
No Summary
```c#
implicit float =( TimeSince ts) 
```
No Summary
```c#
implicit TimeSince =( float ts) 
```
No Summary
## Referencing Members

```c#
TimeSince = NavPath.Age { get; } 
```
```c#
TimeSince = WaterController.TimeSinceLastEffect
```
```c#
TimeSince = BaseWeapon.TimeSincePrimaryAttack { get; set; } 
```
```c#
TimeSince = BaseWeapon.TimeSinceSecondaryAttack { get; set; } 
```
