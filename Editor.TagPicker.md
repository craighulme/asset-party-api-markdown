# TagPicker

## 
```c#
Derives from Widget
```

## Summary

Offers a popup menu with a number of "tags" when you can then select
## Constructors

```c#
TagPicker( Widget parent = null) 
```
No Summary
## Properties

```c#
HashSet<string> ActiveTags { get; set; } 
```
No Summary
```c#
HashSet<string> ExcludedTags { get; set; } 
```
No Summary
```c#
string Icon { get; set; } 
```
No Summary
```c#
Action OnValueChanged { get; set; } 
```
No Summary
```c#
List<Option> Options { get; } 
```
No Summary
```c#
bool ShowSelectAll { get; set; } 
```
Show a button to select all?
```c#
Layout TagsLayout { get; set; } 
```
No Summary
```c#
ToolButton ToolButton { get; protected set; } 
```
No Summary
## Methods

```c#
void Rebuild( ) 
```
No Summary
```c#
void Set( string incomingTag, bool b) 
```
No Summary
```c#
void SetExcluded( string incomingTag, bool b) 
```
No Summary
```c#
void Toggle( string incomingTag) 
```
No Summary
```c#
void ToggleExcluded( string incomingTag) 
```
No Summary
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
## Nested Types

