# ServerRow

## ```c#
Derives from Panel
```

## Summary

OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
## Constructors

```c#
ServerRow( ) 
```
No Summary
## Fields

```c#
Entry Server
```
No Summary
```c#
bool ShowGame
```
No Summary
## Properties

```c#
Action<Entry> OnSelected { get; set; } 
```
No Summary
## Methods

```c#
void Refresh( ) 
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
