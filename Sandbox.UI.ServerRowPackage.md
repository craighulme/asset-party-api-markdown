# ServerRowPackage

## ```c#
Derives from Panel
```

## Summary

OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
## Constructors

```c#
ServerRowPackage( ) 
```
No Summary
## Fields

```c#
string Ident
```
No Summary
```c#
Package Package
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
