# RealTimeSince

## 
```c#
Implements IEquatable<RealTimeSince>
```

## Summary

A convenience struct to easily measure time since an event last happened, based onRealTime.GlobalNow.Typical usage would see you assigning 0 to a variable of this type to reset the timer.
Then the struct would return time since the last reset. i.e.:RealTimeSince lastUsed = 0;
if ( lastUsed > 10 ) { /*Do something*/ }
## Properties

```c#
double Absolute { get; } 
```
Time at which the timer reset happened, based onRealTime.GlobalNow.
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
override bool Equals( RealTimeSince o) 
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
bool ==( RealTimeSince left, RealTimeSince right) 
```
No Summary
```c#
bool >( in RealTimeSince ts, float f) 
```
No Summary
```c#
bool >( in RealTimeSince ts, int f) 
```
No Summary
```c#
bool >=( in RealTimeSince ts, float f) 
```
No Summary
```c#
bool >=( in RealTimeSince ts, int f) 
```
No Summary
```c#
bool !=( RealTimeSince left, RealTimeSince right) 
```
No Summary
```c#
bool <( in RealTimeSince ts, float f) 
```
No Summary
```c#
bool <( in RealTimeSince ts, int f) 
```
No Summary
```c#
bool <=( in RealTimeSince ts, float f) 
```
No Summary
```c#
bool <=( in RealTimeSince ts, int f) 
```
No Summary
```c#
implicit float =( RealTimeSince ts) 
```
No Summary
```c#
implicit RealTimeSince =( float ts) 
```
No Summary
## Referencing Members

```c#
abstract RealTimeSince = IVoice.LastHeard { get; set; } 
```
```c#
RealTimeSince = PhysicsBody.LastWaterEffect { get; set; } 
```
```c#
RealTimeSince = ChatEntry.TimeSinceBorn
```
```c#
RealTimeSince = LoaderFullScreen.timeSinceShown
```
