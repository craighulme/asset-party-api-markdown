# LogicEntity

## 
```c#
Derives from Entity
```

## Summary

A logic entity that allows to do a multitude of logic operations with Map I/O.TODO: This is a stop-gap solution and may be removed in the future in favor of "map blueprints" or node based Map I/O.
## Constructors

```c#
LogicEntity( ) 
```
No Summary
## Properties

```c#
bool Enabled { get; set; } 
```
The (initial) enabled state of the logic entity.
```c#
protected Output OnEqual { get; set; } 
```
Fired when the value given to "CompareInput" or Variable A ("Compare" input) matches our Variable B.
```c#
protected Output OnGreaterThan { get; set; } 
```
Fired when the value given to "CompareInput" or Variable A ("Compare" input) is greater than our Variable B.
```c#
protected Output OnLessThan { get; set; } 
```
Fired when the value given to "CompareInput" or Variable A ("Compare" input) is less than our Variable B.
```c#
protected Output OnMapSpawn { get; set; } 
```

```c#
protected Output OnNotEqual { get; set; } 
```
Fired when the value given to "CompareInput" or Variable A ("Compare" input) is NOT equal our Variable B.
```c#
protected Output OnTrigger { get; set; } 
```
Fired when the this entity receives the "Trigger" input.
```c#
float VariableA { get; set; } 
```
The (initial) value for Variable A
```c#
float VariableB { get; set; } 
```
The (initial) value for Variable B
## Methods

```c#
void Compare( ) 
```
Compares Variable A to Variable B and fires the appropriate output.
```c#
void CompareInput( float input) 
```
Compares the given number to Variable B and fires the appropriate output.
```c#
void Disable( ) 
```
Disables the entity, so that it would not fire any outputs.
```c#
void Enable( ) 
```
Enables the entity.
```c#
void OnMapSpawnEvent( ) 
```
Fired after all map entities have spawned, even if it is disabled.
```c#
void SetVariableA( float input) 
```
Sets the Variable A and fires appropriate outputs.
```c#
void SetVariableB( float input) 
```
Sets the Variable B and fires appropriate outputs.
```c#
void Toggle( ) 
```
Toggles the enabled state of the entity.
```c#
void Trigger( ) 
```
Trigger the "OnTrigger" output.
