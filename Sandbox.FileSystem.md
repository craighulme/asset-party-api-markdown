# FileSystem

## Is static
Derives from object

## Summary

A filesystem that can be accessed by the game.
## Properties

```c#
static BaseFileSystem Data { get; } 
```
A subset ofFileSystem.OrganizationDatafor custom gamemode data.
```c#
static BaseFileSystem Mounted { get; } 
```
All mounted content.
```c#
static BaseFileSystem OrganizationData { get; } 
```
A filesystem for custom data, per gamemode's organization.
## Methods

```c#
static string NormalizeFilename( string filepath) 
```
Normalizes given file path so the game's filesystem can understand it. Fixes slashes and lowercases the file path.
