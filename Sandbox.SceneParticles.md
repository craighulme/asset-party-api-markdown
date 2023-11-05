# SceneParticles

## Derives from SceneObject

## Summary

A SceneObject used to render particles.
We need to be careful with what we do here, because this object is created for in-engine particles
as well as custom scene object particles.
With custom particles there's no automatic Simulate, or deletion.. You're completely on your own. This
is perhaps a good thing though, it's maybe what you want to happen. To be completely isolated and completely
in control. But at the same time maybe it's not and it's something we need to sort out.
## Constructors

```c#
SceneParticles( SceneWorld world, string particleSystem) 
```
Create scene particles.
```c#
SceneParticles( SceneWorld world, ParticleSystem particleSystem) 
```
Create scene particles.
## Properties

```c#
int ActiveParticlesSelf { get; } 
```
The amount of particles
```c#
int ActiveParticlesTotal { get; } 
```
The amount of particles including child systems
```c#
bool EmissionStopped { get; set; } 
```
Stop (or start) the particle system emission.
```c#
bool Finished { get; } 
```
True if particle system has reached the end
```c#
int MaximumParticles { get; } 
```
The total allowed particle count
```c#
bool RenderParticles { get; set; } 
```
Whether to render the particles or not.
```c#
float SimulationTime { get; set; } 
```
Get or set the simulation time
## Methods

```c#
void Emit( int count) 
```
Manually emit a bunch of particles
```c#
Vector3 GetControlPointPosition( int index) 
```
Returns the position set on a given control point.
```c#
bool IsControlPointSet( int index) 
```
Whether given control point has any data set.
```c#
void SetControlPoint( int i, Vector3 position) 
```
Set position on given control point.
```c#
void SetControlPoint( int i, Rotation rotation) 
```
Set rotation on given control point.
```c#
void SetControlPoint( int i, Transform transform) 
```
Set transform on given control point.
```c#
void SetControlPoint( int i, ParticleSnapshot snapshot) 
```
Set snapshot on given control point.
```c#
void Simulate( float f) 
```
Simulate the particles for given amount of time.
