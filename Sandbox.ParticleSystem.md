# ParticleSystem

## 
```c#
Derives from Resource
```

## Summary

A particle effect system that allows for complex visual effects, such as
explosions, muzzle flashes, impact effects, etc.
## Properties

```c#
int ChildCount { get; } 
```
How many child particle systems do we have
```c#
bool IsError { get; } 
```
Whether the particle system is invalid, or has not yet loaded.
```c#
string Name { get; } 
```
Particle system file name.
## Methods

```c#
static ParticleSystem Load( string filename) 
```
Loads a particle system from given file.
```c#
ParticleSystem GetChild( int index) 
```
Returns child particle at given index.
```c#
override string ToString( ) 
```
OverridesObject.ToString
