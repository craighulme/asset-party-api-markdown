# FeatureBox

## 
```c#
Derives from Widget
```

## Summary

OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
## Constructors

```c#
FeatureBox( Widget parent, string title, float margin = 8) 
```
No Summary
## Properties

```c#
Widget Content { get; } 
```
No Summary
```c#
Widget Header { get; } 
```
No Summary
```c#
string Title { get; set; } 
```
No Summary
```c#
bool Value { get; set; } 
```
No Summary
## Methods

```c#
void Add( Widget widget) 
```
No Summary
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
