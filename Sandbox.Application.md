# Application

## 
```c#
Derives from object
```

## Summary

True if running with the tools or editor attached
## Properties

```c#
static bool IsEditor { get; } 
```
True if running with the tools or editor attached
```c#
static bool IsHeadless { get; } 
```
True if running as a background task, or terminal, like a dedicated server.
```c#
static bool IsUnitTest { get; } 
```
True if we're running the engine as part of a unit test
## Methods

```c#
static void InitUnitTest( ) 
```
Called from unit test projects to initialize the engine
