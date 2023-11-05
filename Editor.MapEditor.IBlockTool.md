# IBlockTool

## 
```c#
Is interface
```

## Summary

Interface for the addon layer to implement, this is called from native Hammer.
## Properties

```c#
static IBlockTool Instance { get; set; } 
```
No Summary
```c#
static bool OrientPrimitives { get; set; } 
```
No Summary
```c#
abstract PrimitiveBuilder Current { get; set; } 
```
No Summary
```c#
abstract string EntityOverride { get; set; } 
```
No Summary
```c#
abstract bool InProgress { get; set; } 
```
No Summary
## Methods

```c#
static void UpdateTool( ) 
```
Tells the tool a parameter has changed and that we should redraw.
```c#
abstract Widget BuildUI( ) 
```
No Summary
