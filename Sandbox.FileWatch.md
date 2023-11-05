# FileWatch

## Derives from object
Implements IDisposable

## Summary

Watch folders, dispatch events on changed files
## Fields

```c#
List<string> watchFiles
```
No Summary
## Properties

```c#
List<string> Changes { get; } 
```
No Summary
```c#
bool Enabled { get; set; } 
```
No Summary
## Methods

```c#
static void Tick( ) 
```
No Summary
```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.Dispose
## Events

```c#
OnChangedFile( string obj) 
```
Called for each file changed
```c#
OnChanges( FileWatch obj) 
```
Called once per batch of files changed
