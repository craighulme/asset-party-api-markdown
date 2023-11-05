# ExplosionEntity

## Derives from Entity

## Summary

An entity that creates an explosion at its center.
## Constructors

```c#
ExplosionEntity( ) 
```
No Summary
## Properties

```c#
float Damage { get; set; } 
```
Damage the explosion should do at the center. The damage will reduce the farther the target is from the center of the explosion.
```c#
float ForceScale { get; set; } 
```
Scale explosion induced physics forces by this amount.
```c#
string ParticleOverride { get; set; } 
```
If set, will override the default explosion particle effect.
```c#
float Radius { get; set; } 
```
Radius of the explosion.
```c#
bool RemoveOnExplode { get; set; } 
```
Delete this entity when it is triggered via the Explode input?
```c#
string SoundOverride { get; set; } 
```
If set, will override the default explosion sound.
## Methods

```c#
void Explode( Entity activator) 
```
Perform the explosion.
