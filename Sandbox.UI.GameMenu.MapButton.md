# MapButton

## 
```c#
Derives from Panel
```

## Summary

OverridesPanel.BuildHashBy overriding this you can return a hash of variables used by the Razor layout, which
will cause a rebuild when changed. This is useful when your layout uses a global variable
because by adding it to a HashCode.Combine here you can easily trigger a build when it changes.
## Constructors

```c#
MapButton( ) 
```
No Summary
## Properties

```c#
string MapIdent { get; set; } 
```
No Summary
```c#
Package MapPackage { get; set; } 
```
No Summary
```c#
Action OnClicked { get; set; } 
```
No Summary
## Methods

```c#
protected override int BuildHash( ) 
```
OverridesPanel.BuildHashBy overriding this you can return a hash of variables used by the Razor layout, which
will cause a rebuild when changed. This is useful when your layout uses a global variable
because by adding it to a HashCode.Combine here you can easily trigger a build when it changes.
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
