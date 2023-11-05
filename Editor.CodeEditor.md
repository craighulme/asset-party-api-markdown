# CodeEditor

## 
```c#
Derives from object
```

## Summary

For opening source code files in whatever code editor the user has selected.
## Properties

```c#
static ICodeEditor Current { get; set; } 
```
No Summary
```c#
static string Title { get; } 
```
No Summary
## Methods

```c#
static string AddonSolutionPath( ) 
```
No Summary
```c#
static void BuildMenu( ) 
```
No Summary
```c#
static void BuildPreferences( PropertySheet sheet) 
```
No Summary
```c#
static string FindSolutionFromPath( string path) 
```
Finds a .sln this path belongs to, this is pretty much entirely for internal usage to open engine slns
```c#
static void OpenAddon( LocalProject addon) 
```
No Summary
```c#
static void OpenFile( string path, int? line = null, int? column = null) 
```
Opens a file in the current editor, optionally at a line and column.
```c#
static void OpenSolution( ) 
```
Open the solution of all s&box projects
