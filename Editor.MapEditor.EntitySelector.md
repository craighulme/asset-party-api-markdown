# EntitySelector

## ```c#
Derives from Widget
```

## Summary

OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
## Constructors

```c#
EntitySelector( Widget parent, bool isPathTool = false) 
```
No Summary
## Properties

```c#
bool CollapsedSidebar { get; set; } 
```
No Summary
```c#
string CookieCollapsedSidebar { get; } 
```
No Summary
```c#
string CookiePreferClassNames { get; } 
```
No Summary
```c#
string LastTabCookieKey { get; } 
```
No Summary
```c#
bool PreferClassNames { get; set; } 
```
No Summary
```c#
string SelectedEntity { get; set; } 
```
No Summary
## Methods

```c#
IEnumerable<IGrouping<string, MapClass>> GetItems( ) 
```
No Summary
```c#
void SwitchTab( string category) 
```
No Summary
```c#
void UpdateList( ) 
```
No Summary
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
