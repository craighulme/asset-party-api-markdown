# ServerListPanel

## 
```c#
Derives from Panel
```

## Summary

OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
## Constructors

```c#
ServerListPanel( ) 
```
No Summary
## Properties

```c#
string FilterByGame { get; set; } 
```
No Summary
```c#
Action<Entry> OnSelected { get; set; } 
```
No Summary
```c#
bool ShowEmpty { get; set; } 
```
No Summary
```c#
bool ShowFull { get; set; } 
```
No Summary
```c#
bool ShowGame { get; set; } 
```
No Summary
```c#
string TextFilter { get; set; } 
```
No Summary
## Methods

```c#
Task Refresh( ) 
```
No Summary
```c#
protected override void BuildRenderTree( RenderTreeBuilder __builder) 
```
OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
```c#
protected override string GetRenderTreeChecksum( ) 
```
OverridesPanel.GetRenderTreeChecksumOverridden/implemented by Razor templating, contains render tree checksum to determine when the render tree content has changed.
```c#
protected override void OnParametersSet( ) 
```
OverridesPanel.OnParametersSetCalled after all templated panel binds have been set.
