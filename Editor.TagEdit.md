# TagEdit

## Derives from Widget

## Summary

A text entry that automatically breaks the input into tags
## Constructors

```c#
TagEdit( Widget parent = null) 
```
No Summary
## Properties

```c#
List<Func<string, TagDetail>> Convertors { get; init; } 
```
No Summary
```c#
LineEdit LineEdit { get; set; } 
```
No Summary
```c#
Action OnEdited { get; set; } 
```
Called when the contents are edited, either by typing or removing a tag
```c#
string Value { get; set; } 
```
Outputs the tags followed by any unswallowed text
```c#
string ValueTags { get; set; } 
```
Like Value but only outputs accepted tags
## Methods

```c#
void TryConvertTags( ) 
```
No Summary
## Nested Types

