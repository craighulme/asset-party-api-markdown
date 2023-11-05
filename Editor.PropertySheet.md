# PropertySheet

## Derives from Widget

## Summary

Adds a multi-lineEditor.TextEditthat binds to a dictionary value.
## Constructors

```c#
PropertySheet( Widget parent) 
```
No Summary
## Fields

```c#
Action PropertyUpdated
```
No Summary
## Properties

```c#
Layout BodyLayout { get; } 
```
No Summary
```c#
bool IncludeHeader { get; set; } 
```
No Summary
```c#
object Target { get; set; } 
```
No Summary
```c#
SerializedObject TargetObject { get; set; } 
```
No Summary
```c#
object Value { get; set; } 
```
No Summary
## Methods

```c#
static string BuildHierarchyName( Widget widget) 
```
No Summary
```c#
TextEdit AddDictionaryTextEdit( Dictionary<string, object> target, string targetName, string defaultValue, string title = null) 
```
Adds a multi-lineEditor.TextEditthat binds to a dictionary value.
```c#
LineEdit AddLineEdit( string title, string value) 
```
No Summary
```c#
Widget AddProperty( object target, string targetName) 
```
No Summary
```c#
T AddRow<T,>( T row, string name = null) 
```
No Summary
```c#
T AddRow<T,>( string title, T widget) 
```
No Summary
```c#
T AddRow<T,>( T row, PropertyInfo prop) 
```
No Summary
```c#
void AddSectionHeader( string name) 
```
No Summary
```c#
TextEdit AddTextEdit( string title, string value) 
```
No Summary
```c#
ExpandGroup CreateExpander( string title) 
```
No Summary
```c#
override void ChildValuesChanged( Widget source) 
```
OverridesWidget.ChildValuesChanged
## Inheriting Types

