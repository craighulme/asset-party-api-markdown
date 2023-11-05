# MapClassVariable

## Derives from object

## Summary

Represents a variable.
## Constructors

```c#
MapClassVariable( ) 
```
No Summary
## Properties

```c#
object DefaultValue { get; set; } 
```
Default value for this variable.
```c#
string Description { get; set; } 
```
Description for this variable.
```c#
string GroupName { get; set; } 
```
Category or group for this variable.
```c#
string LongName { get; set; } 
```
The user friendly name for UI.
```c#
Dictionary<string, string> Metadata { get; set; } 
```
General purpose key-value store to alter functionality of UI, map compilation, editor helpers, etc.
```c#
string Name { get; set; } 
```
The internal name.
```c#
Type PropertyType { get; set; } 
```
Data type for this variable.
```c#
string PropertyTypeOverride { get; set; } 
```
Internal, used to override the type to one the tools understand.
## Methods

```c#
override string ToString( ) 
```
OverridesObject.ToString
