# ConsoleSystem

## Is static
Derives from object

## Summary

Get a convar value as a string
## Methods

```c#
static string GetValue( string name, string defaultValue = null) 
```
Get a convar value as a string
```c#
static float GetValueFloat( string name, float defaultValue = 0) 
```
Get a convar value as an float if possible.
```c#
static int GetValueInt( string name, int defaultValue = 0) 
```
Get a convar value as an integer if possible.
```c#
static void Run( string command) 
```
Run this command. This should be a single command.
```c#
static void SetValue( string name, object value) 
```
Try to set a console variable. You will only be able to set variables that you have permission to set.
