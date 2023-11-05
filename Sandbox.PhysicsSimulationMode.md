# PhysicsSimulationMode

## 
```c#
Derives from Enum
```

## Summary

Physics simulation mode. For use withPhysicsWorld.SimulationMode.
## Fields

```c#
static PhysicsSimulationMode Continuous = 1
```
Continuous collision detection. This is the default mode.
```c#
static PhysicsSimulationMode Discrete = 0
```
Discrete collision detection.
In this mode physics bodies can fly through thin walls when moving very quickly, but it is has better performance.
## Referencing Members

```c#
PhysicsSimulationMode = PhysicsWorld.SimulationMode { get; set; } 
```
```c#
PhysicsSimulationMode = PhysicsSettings.SimulationMode { get; set; } 
```
