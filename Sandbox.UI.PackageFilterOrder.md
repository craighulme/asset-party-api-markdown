# PackageFilterOrder

## Derives from Panel

## Summary

OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
## Constructors

```c#
PackageFilterOrder( ) 
```
No Summary
## Properties

```c#
Action<string> OnChange { get; set; } 
```
No Summary
```c#
SortOrder[] Orders { get; set; } 
```
No Summary
```c#
string Value { get; set; } 
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
