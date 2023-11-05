# PackageFilters

## Derives from Panel

## Summary

OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
## Constructors

```c#
PackageFilters( ) 
```
No Summary
## Properties

```c#
Action<string> OnChange { get; set; } 
```
No Summary
```c#
string Query { get; set; } 
```
No Summary
```c#
FindResult Result { get; set; } 
```
No Summary
```c#
string SearchString { get; set; } 
```
No Summary
## Methods

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
```c#
override void Tick( ) 
```
OverridesPanel.TickCalled every frame. This is your "Think" function.
