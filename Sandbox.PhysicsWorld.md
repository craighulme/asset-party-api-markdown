# PhysicsWorld

## 
```c#
Implements IHandle
```

## Summary

A world in which physics objects exist. You can create your own world but you really don't need to. A world for the map is created clientside and serverside automatically.
## Constructors

```c#
PhysicsWorld( ) 
```
Create a new physics world. You should only do this if you want to simulate an extra world for some reason.
## Properties

```c#
float AirDensity { get; set; } 
```
Air density of this physics world, for things like air drag.
```c#
PhysicsBody Body { get; } 
```
The body of this physics world.
```c#
Vector3 Gravity { get; set; } 
```
Access the world's current gravity.
```c#
PhysicsGroup Group { get; } 
```
The physics group of this physics world. A physics world will contain only 1 body.
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
PhysicsTraceBuilder Trace { get; } 
```
Raytrace against this world
```c#
int VelocityIterations { get; set; } 
```
Used for constraints (joints). Higher values should result in more accurate simulation (TODO: Confirm this)
## Methods

```c#
void Delete( ) 
```
Delete this world and all objects inside. Will throw an exception if you try to delete a world that you didn't manually create.
```c#
void SetCollisionRules( CollisionRules rules) 
```
Used internally to set collision rules from gamemode's project settings.
You shouldn't need to call this yourself.
```c#
PhysicsGroup SetupPhysicsFromModel( Model model, PhysicsMotionType motionType) 
```
Temp function for creating model physics until entity system handles it
```c#
PhysicsGroup SetupPhysicsFromModel( Model model, Transform transform, PhysicsMotionType motionType) 
```
Temp function for creating model physics until entity system handles it
```c#
void Step( float time) 
```
Step simulation of this physics world. You can only do this on physics worlds that you manually create.
```c#
void Step( float time, int subSteps) 
```
Step simulation of this physics world. You can only do this on physics worlds that you manually create.
