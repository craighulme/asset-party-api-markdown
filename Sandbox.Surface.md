# Surface

## 
```c#
Derives from GameResource
```

## Summary

A physics surface. This is applied to eachPhysicsShapeand controls its physical properties and physics related sounds.
## Constructors

```c#
Surface( ) 
```
No Summary
## Properties

```c#
string AudioMaterial { get; set; } 
```
Defines the audio properties of this surface for Steam Audio
```c#
string BaseSurface { get; set; } 
```
Filepath of the base surface. UseSetBaseSurfaceandGetBaseSurface.
```c#
float BounceThreshold { get; set; } 
```
Velocity threshold, below which objects will not bounce due to their elasticity.
```c#
BreakablesInfo Breakables { get; set; } 
```
Breakable info for this surface material.
```c#
float Dampening { get; set; } 
```
Currently unused and does nothing.
```c#
float Density { get; set; } 
```
Density of this surface material. This affects things like automatic mass calculation.
Density is in kg/m^3.
```c#
string Description { get; set; } 
```
A concise description explaining what this surface property should be used for.
```c#
float Elasticity { get; set; } 
```
Controls bounciness.
```c#
float Friction { get; set; } 
```
Friction of this surface material.
```c#
ImpactEffectData ImpactEffects { get; set; } 
```
Impact effects of this surface material.
```c#
int Index { get; } 
```
No Summary
```c#
uint NameHash { get; } 
```
No Summary
```c#
ScrapeEffectData ScrapeEffects { get; set; } 
```
Scrape effects of this surface material.
```c#
SoundData Sounds { get; set; } 
```
Sounds associated with this surface material.
```c#
string Tags { get; set; } 
```
A list of tags as one string.
```c#
float Thickness { get; set; } 
```
If above 0, the object is considered hollow, and its auto generated mass is affected accordingly.
Thickness is in inches.
## Methods

```c#
static Surface FindByName( string name) 
```
Returns a Surface from its name, or null
```c#
Surface GetBaseSurface( ) 
```
Returns the base surface of this surface, or null if we are the default surface.
```c#
string GetRandomGib( ) 
```
Returns a random gib taking into account base surface.
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
Do we have a tag?
```c#
void SetBaseSurface( string name) 
```
Sets the base surface by name.
```c#
override string ToString( ) 
```
OverridesObject.ToString
## Extensions

```c#
Particles DoBulletImpact( TraceResult tr) 
```
Create a particle effect and play an impact sound for this surface being hit by a bullet
```c#
void DoFootstep( Entity ent, TraceResult tr, int foot, float volume) 
```
Create a footstep effect
## Nested Types

