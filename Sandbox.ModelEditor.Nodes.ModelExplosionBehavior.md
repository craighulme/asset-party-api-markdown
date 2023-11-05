# ModelExplosionBehavior

## Derives from object

## Summary

Defines the model as explosive. Support for this depends on the entity.
## Constructors

```c#
ModelExplosionBehavior( ) 
```
No Summary
## Properties

```c#
float Damage { get; set; } 
```
Amount of damage to do at the center on the explosion. It will falloff over distance.
```c#
string Effect { get; set; } 
```
Particle effect override for when the problem explodes.
```c#
float Force { get; set; } 
```
Scale of the force applied to entities damaged by the explosion and the models break pieces.
```c#
float Radius { get; set; } 
```
Range of explosion's damage.
```c#
string Sound { get; set; } 
```
Sound override for when the prop explodes.
