# Hitbox

## ```c#
Derives from ValueType
```

## Summary

Hitboxes are used with Traces, and given by TraceResult if using Trace.UseHitboxes.
We're storing as much data here as string tokens. Any public method in this class should be treated as a heavy operation.
## Methods

```c#
string GetName( ) 
```
Grab the name of the hitbox, please note that internally we store this as a string token, so using this frequently is ill advised.
```c#
bool HasAllTags( string[] tags) 
```
Do we have all the tags on this hitbox?
```c#
bool HasAnyTags( string[] tags) 
```
Do we have all the tags on this hitbox?
```c#
bool HasTag( string tag) 
```
Do we have a tag on this hitbox?
## Referencing Members

```c#
Hitbox = DamageInfo.Hitbox { get; set; } 
```
```c#
Hitbox = TraceResult.Hitbox
```
