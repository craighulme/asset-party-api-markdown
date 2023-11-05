# AddonManifest

## ```c#
Derives from object
```

## Summary

This really exists only to dissallow dangerous extensions like .exe etc.
So feel free to add anything non dangerous to this list.
## Constructors

```c#
AddonManifest( ) 
```
No Summary
## Fields

```c#
static string[] DissallowedExtensions
```
This really exists only to dissallow dangerous extensions like .exe etc.
So feel free to add anything non dangerous to this list.
```c#
List<string> Errors
```
No Summary
## Properties

```c#
List<ProjectFile> Assets { get; set; } 
```
No Summary
```c#
HashSet<string> CodePackageReferences { get; } 
```
List of packages that the code references
```c#
string Description { get; set; } 
```
No Summary
```c#
string Summary { get; set; } 
```
No Summary
## Methods

```c#
static bool LooseFileAllowed( string file) 
```
No Summary
```c#
Task AddTextFile( string contents, string relativePath) 
```
No Summary
```c#
Task BuildFrom( LocalProject addon, IProgress progress = null, CancellationToken cancel = null) 
```
No Summary
```c#
ProjectFile FindAsset( string relativePath) 
```
No Summary
```c#
string ToJson( ) 
```
No Summary
