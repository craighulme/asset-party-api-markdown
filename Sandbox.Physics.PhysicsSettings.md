# PhysicsSettings

## 
```c#
Derives from object
```

## Summary

Used by project settings to describe physics settings. This is Json serializable and is synced
with the client via the string tables.
## Constructors

```c#
PhysicsSettings( ) 
```
No Summary
## Properties

```c#
float AirDensity { get; set; } 
```
Air density of this physics world, for things like air drag.
```c#
Vector3 Gravity { get; set; } 
```
Access the world's current gravity.
```c#
int PositionIterations { get; set; } 
```
Used for constraints (joints). Higher values should result in more accurate simulation (TODO: Confirm this)
```c#
PhysicsSimulationMode SimulationMode { get; set; } 
```
Physics simulation mode. SeeSandbox.PhysicsSimulationModefor explanation of each mode.
```c#
bool SleepingEnabled { get; set; } 
```
If true then bodies will be able to sleep after a period of inactivity
```c#
int SoftBodyIterations { get; set; } 
```
Does not appear to be used for anything.
```c#
int SoftBodySubsteps { get; set; } 
```
Does not appear to be used for anything.
```c#
int SubSteps { get; set; } 
```
If you're seeing objects go through other objects or you have a low tickrate, you might want to increase the number of physics substeps.
This breaks physics steps down into this many substeps. The default is 1 and works pretty good.
Be aware that the number of physics ticks per second is going to be tickrate * substeps.
So if you're ticking at 90 and you have SubSteps set to 1000 then you're going to do 90,000 steps per second. So be careful here.
```c#
float TimeScale { get; set; } 
```
Physics time scale. 0.5 is half speed, 1 is full speed, etc.
```c#
int VelocityIterations { get; set; } 
```
Used for constraints (joints). Higher values should result in more accurate simulation (TODO: Confirm this)
## Methods

```c#
void Clean( ) 
```
Applies sane limits on values of these settings.
