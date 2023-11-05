# LifeState

## ```c#
Derives from Enum
```

## Summary

Alive as normal
## Fields

```c#
static LifeState Alive = 0
```
Alive as normal
```c#
static LifeState Dead = 2
```
Dead, lying still
```c#
static LifeState Dying = 1
```
Playing a death animation
```c#
static LifeState Respawnable = 3
```
Can respawn, usually waiting for some client action to respawn
```c#
static LifeState Respawning = 4
```
Is in the process of respawning
## Referencing Members

```c#
LifeState = Entity.LifeState { get; set; } 
```
