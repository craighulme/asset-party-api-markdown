# GameSetting

## ```c#
Derives from object
```

## Summary

A game setting based on a ConVar that has been set up in the games Project Settings.
## Constructors

```c#
GameSetting( ) 
```
No Summary
## Properties

```c#
GameSettingChoice[] Choices { get; set; } 
```
An array of possible choices for this game setting.
```c#
string ConVarName { get; set; } 
```
The ConVar that this setting will change.
```c#
string DefaultValue { get; set; } 
```
The default value the ConVar will be set to.
```c#
string Description { get; set; } 
```
Some useful information describing what this game setting does.
```c#
string DisplayName { get; set; } 
```
The name that is displayed in the game lobby.
```c#
GameSettingType DisplayType { get; set; } 
```
What kind of variable the game setting represents. This decides how the setting is represented visually.
```c#
string Group { get; set; } 
```
If you want to group your settings
```c#
float Maximum { get; set; } 
```
The maximum number value for the ConVar.
```c#
float Minimum { get; set; } 
```
The minimum number value for the ConVar.
```c#
float Step { get; set; } 
```
The incremental value to use for sliders.
## Methods

```c#
bool IsValidValue( string value) 
```
Whether or not the specified string value is valid for this game setting.
## Nested Types

