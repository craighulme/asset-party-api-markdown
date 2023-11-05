# ModelDoorSounds

## 
```c#
Derives from object
```

## Summary

Sounds to be used by ent_door if it does not override sounds.
## Constructors

```c#
ModelDoorSounds( ) 
```
No Summary
## Properties

```c#
string CloseSound { get; set; } 
```
Sound to play when the door starts to close.
```c#
string FullyClosedSound { get; set; } 
```
Sound to play when the door reaches it's fully closed position.
```c#
string FullyOpenSound { get; set; } 
```
Sound to play when the door reaches it's fully open position.
```c#
string LockedSound { get; set; } 
```
Sound to play when the door is attempted to be opened, but is locked.
```c#
string MovingSound { get; set; } 
```
Sound to play while the door is moving. Typically this should be looping or very long.
```c#
string OpenSound { get; set; } 
```
Sound to play when the door starts to open.
