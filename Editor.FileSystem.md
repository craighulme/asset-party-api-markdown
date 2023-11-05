# FileSystem

## ```c#
Derives from object
```

## Summary

A filesystem that can be accessed by the game.
## Properties

```c#
static BaseFileSystem Cloud { get; } 
```
A tools only filesystem that is mounted when developing. We download files from Asset Party right into this
filesystem. The aim of this filesystem should be that we should be able to wipe it at any time and restore it
from the cloud and everything should still work.
```c#
static BaseFileSystem Content { get; } 
```
Content from active addons (and content paths)
```c#
static BaseFileSystem Mounted { get; } 
```
Paths from tool addons which are mounted.
```c#
static BaseFileSystem Root { get; } 
```
Root of the game's folder.
```c#
static BaseFileSystem Temporary { get; } 
```
The /.source2/ folder for temporary files and caches.
```c#
static BaseFileSystem WebCache { get; } 
```
The /.source2/http/ folder.
## Methods

```c#
static void SuppressNextHotload( ) 
```
Stop the game from triggering a hotload for this file - because presumably you have
already reloaded it.
