# PackageList

## 
```c#
Derives from Panel
```

## Summary

OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
## Constructors

```c#
PackageList( ) 
```
No Summary
## Properties

```c#
Package[] FoundPackages { get; set; } 
```
No Summary
```c#
Action<FindResult> OnResult { get; set; } 
```
No Summary
```c#
Action<Package> OnSelected { get; set; } 
```
No Summary
```c#
string Query { get; set; } 
```
No Summary
```c#
bool ShowFilters { get; set; } 
```
No Summary
```c#
int Skip { get; set; } 
```
No Summary
```c#
int Take { get; set; } 
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
protected override Task OnParametersSetAsync( ) 
```
OverridesPanel.OnParametersSetAsyncCalled after all templated panel binds have been set.
