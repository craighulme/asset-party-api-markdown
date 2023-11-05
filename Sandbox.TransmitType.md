# TransmitType

## ```c#
Derives from Enum
```

## Summary

Entity transmit mode, dictates when entity will be networked to clients.
## Fields

```c#
static TransmitType Always = 1
```
Transmit always, no matter what.
```c#
static TransmitType Default = 0
```
Engine will decide when to transmit the entity.
```c#
static TransmitType Never = 2
```
Do not transmit, ever.
```c#
static TransmitType Owner = 4
```
Inherit the transmit type from parent or owner.
```c#
static TransmitType Pvs = 3
```
Entity will be networked if it's in a client (or its Pawn's) PVS
## Referencing Members

```c#
TransmitType = Entity.Transmit { get; set; } 
```
