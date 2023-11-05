# PackageFilterFacet

## Derives from Panel

## Summary

OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
## Constructors

```c#
PackageFilterFacet( ) 
```
No Summary
## Properties

```c#
Facet Facet { get; set; } 
```
No Summary
```c#
Action<Facet, string> OnChange { get; set; } 
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
