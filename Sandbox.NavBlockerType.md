# NavBlockerType

## ```c#
Derives from Enum
```

## Summary

An obstacle that marks entire areas it intersects with as blocked.
## Fields

```c#
static NavBlockerType AREA = 2
```
An obstacle that marks entire areas it intersects with as blocked.
```c#
static NavBlockerType AVOID = 1
```
An "avoidance" obstacle. Places a height-based obstruction onto nav areas.
```c#
static NavBlockerType BLOCK = 3
```
An obstacle that blocks nav, possibly cutting nav or triggering dynamic generation.
## Referencing Members

```c#
NavBlocker.NavBlocker( NavBlockerType ) 
```
