# WaterEffectComponent

## Derives from EntityComponent
Implements ISingletonComponent

## Summary

Added to an entity when it enters water. Removed when it leaves water.
## Constructors

```c#
WaterEffectComponent( ) 
```
No Summary
## Properties

```c#
Entity WaterEntity { get; set; } 
```
The water entity we're inside of
```c#
float WaterLevel { get; set; } 
```
How submerged we are in the water. 0 is none, 1 is over our head.
