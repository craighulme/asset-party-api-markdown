# StyleSheet

## 
```c#
Derives from object
```

## Summary

Releases the filesystem watcher so we won't get file changed events.
## Constructors

```c#
StyleSheet( ) 
```
No Summary
## Fields

```c#
Dictionary<string, KeyFrames> KeyFrames
```
No Summary
```c#
Dictionary<string, string> Variables
```
No Summary
## Properties

```c#
static List<StyleSheet> Loaded { get; } 
```
No Summary
```c#
string FileName { get; } 
```
No Summary
```c#
List<string> IncludedFiles { get; set; } 
```
No Summary
```c#
List<StyleBlock> Nodes { get; set; } 
```
No Summary
## Methods

```c#
static StyleSheet FromFile( string filename, IEnumerable<ValueTuple<string, string>> variables = null) 
```
No Summary
```c#
static StyleSheet FromString( string styles, string filename = "none", IEnumerable<ValueTuple<string, string>> variables = null, bool notices = false) 
```
No Summary
```c#
void AddKeyFrames( KeyFrames frames) 
```
No Summary
```c#
string GetVariable( string name, string defaultValue = null) 
```
No Summary
```c#
void Release( ) 
```
Releases the filesystem watcher so we won't get file changed events.
```c#
string ReplaceVariables( string str) 
```
No Summary
