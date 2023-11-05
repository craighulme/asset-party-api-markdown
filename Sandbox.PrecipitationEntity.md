# PrecipitationEntity

## ```c#
Derives from ModelEntity
```

## Summary

A solid entity that creates rain and snow inside its volume.
## Constructors

```c#
PrecipitationEntity( ) 
```
No Summary
## Properties

```c#
static float DensityScale { get; set; } 
```
Particle density scale for all precipitation entities.
```c#
float Density { get; set; } 
```
Set the Density of the Particle, which will set control point 3 on the particle system.
```c#
float FadingTime { get; set; } 
```
Sets the time particles take to fade in or out when turned on or off
```c#
float InnerFarDistance { get; set; } 
```
How far in front of player's view to place the "far" effect.
```c#
string InnerFarEffect { get; set; } 
```
Particle effect to be placed at "Inner Far Distance" away from the view
```c#
float InnerNearDistance { get; set; } 
```
How far in front of player's view to place the "near" effect.
```c#
string InnerNearEffect { get; set; } 
```
Particle effect to be placed at "Inner Near Distance" away from the view
```c#
bool IsRunning { get; set; } 
```
Sets if the particles are running by default
```c#
string OuterEffect { get; set; } 
```
Particle effect to be placed at the current view's position
```c#
Color ParticleTint { get; set; } 
```
Set the Tint of the Particle, which will set control point 4 on the particle system.
```c#
SpawnType SpawnLocation { get; set; } 
```
Sets where the particles will spawn, around the main camera or around the pawn.
## Methods

```c#
void ChangeDensity( float densitychanged) 
```
Change the particle density.
```c#
void FreezeParticles( ) 
```
Freezes particles in current state.
```c#
void ParticleTimeScale( float particletimescale) 
```
Slow or speed up particles. 1 = normal, 0.5 = half speed, 2 = twice the speed.
```c#
void SetActive( bool isActive) 
```
Turn the volume on or off.
```c#
void SetActive( To toTarget, bool isActive) 
```
Turn the volume on or off.
```c#
void SetParticleState( bool newState) 
```
Enable or disable the particle simulation, i.e. allows pausing the particles.
```c#
void SetParticleState( To toTarget, bool newState) 
```
Enable or disable the particle simulation, i.e. allows pausing the particles.
```c#
void SetParticleTimeScale( float timeScale) 
```
Sets particle time scale.
```c#
void SetParticleTimeScale( To toTarget, float timeScale) 
```
Sets particle time scale.
```c#
void Start( ) 
```
Start the particles.
```c#
void Stop( ) 
```
Stop the particles.
```c#
void UnFreezeParticles( ) 
```
UnFreezes particles if they were previously frozen.
```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
```c#
override void EndTouch( Entity other) 
```
OverridesEntity.EndTouchAn entity has stopped touching this trigger entity. RequiresEnableTouchenabled on this entity.
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
```c#
override void StartTouch( Entity other) 
```
OverridesEntity.StartTouchAn entity has started touching this trigger entity. RequiresEnableTouchenabled on this entity.For solid collisions, seeEntity.OnPhysicsCollision.
## Nested Types

