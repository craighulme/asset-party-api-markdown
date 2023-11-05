# ConsoleSystem

## ```c#
Derives from object
```

## Summary

A library to interact with the Console System.
## Properties

```c#
static IClient Caller { get; } 
```
Returns the player who is calling the command. This will be null
if the command is being called via RCON, or triggered directly
on the server.
## Methods

```c#
static string Build( string command, object[] parameters) 
```
Given a command and parameters, build a coherent command.
```c#
static string GetValue( string name, string defaultValue = null) 
```
Get a console variable's value as a string.
```c#
static void Run( string command) 
```
Run this command. This should be a single command.
```c#
static void Run( string command, object[] arguments) 
```
Run this command, along with the arguments. We'll automatically convert them to strings and handle quoting.
```c#
static void SetValue( string name, object value) 
```
Try to set a console variable. You will only be able to set variables that you have permission to set.
```c#
static void UpdateUserData( string name, object value, bool create = false) 
```
Sends changed Client Data to the server. You shouldn't have to manually call this, it's called automatically by console variables that you mark with the ClientData attribute.
