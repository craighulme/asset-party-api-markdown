# CompilerSettings

## ```c#
Derives from object
```

## Summary

Folders to ignore when walking the tree
## Constructors

```c#
CompilerSettings( ) 
```
No Summary
## Properties

```c#
string DefineConstants { get; set; } 
```
No Summary
```c#
IReadOnlySet<string> DistinctReferences { get; } 
```
No Summary
```c#
HashSet<string> IgnoreFolders { get; set; } 
```
Folders to ignore when walking the tree
```c#
string NoWarn { get; set; } 
```
No Summary
```c#
bool Nullables { get; set; } 
```
No Summary
```c#
Func<string, string> PreProcessSource { get; set; } 
```
Optional function to transform code files before being parsed.
Mainly used by tests, to emulate code changes.
```c#
List<string> References { get; set; } 
```
No Summary
```c#
CompilerReleaseMode ReleaseMode { get; set; } 
```
No Summary
```c#
string RootNamespace { get; set; } 
```
No Summary
```c#
Func<string, bool> SourcePathFilter { get; set; } 
```
Optional predicate to filter which files to compile.
```c#
string WarningsAsErrors { get; set; } 
```
No Summary
## Methods

```c#
void Clean( ) 
```
No Summary
