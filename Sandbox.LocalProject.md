# LocalProject

## Derives from object

## Summary

Represents an on-disk project
painday: rename to Project
## Constructors

```c#
LocalProject( ) 
```
No Summary
## Properties

```c#
static LocalProject CurrentGame { get; } 
```
Currently-loaded game project.
If null, assume that the editor is in Content Mode.
```c#
bool Active { get; set; } 
```
True if this project is active
```c#
bool Broken { get; set; } 
```
True if this project failed to load properly for some reason
```c#
ProjectConfig Config { get; set; } 
```
Configuration of the project.
```c#
Diagnostic[] Diagnostics { get; } 
```
Compiler diagnostics.
```c#
string EditUrl { get; } 
```
The URL to the package's page for editing
```c#
bool HasCompileErrors { get; } 
```
Whether there were any compile errors when last compiling the projects code.
```c#
bool HasCompiler { get; } 
```
Whether the project's code has a compiler assigned.
```c#
bool IsBuiltIn { get; } 
```
If true this project isn't a 'real' project. It's likely a temporary project created with the
intention to configure and publish a single asset.
```c#
bool IsPublished { get; } 
```
Returns true if this project has previously been published. This is kind of a guess though
because all it does is look to see if we have a published package cached with the same ident.
```c#
bool IsTransient { get; } 
```
If true this project isn't a 'real' project. It's likely a temporary project created with the
intention to configure and publish a single asset.
```c#
DateTimeOffset LastOpened { get; set; } 
```
When did the user last open this project?
```c#
Package Package { get; } 
```
The package for this project. This is a mock up of the actual package.
```c#
string Path { get; set; } 
```
Absolute path to the .addon file
```c#
bool Pinned { get; set; } 
```
True if this project is pinned, we'll prioritise it when sorting
```c#
string ViewUrl { get; } 
```
The URL to the package's page for viewing/linking
## Methods

```c#
string GetAssetsPath( ) 
```
Absolute path to the assets folder of the project, ornullif not set.
```c#
string GetCodePath( ) 
```
Absolute path to the code folder of the project.
```c#
string GetRootPath( ) 
```
Absolute path to the location of the.sbprojfile of the project.
## Extensions

```c#
Asset[] GetAssets( ) 
```
Get all assets in this project
