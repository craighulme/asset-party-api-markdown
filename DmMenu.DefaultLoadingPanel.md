# DefaultLoadingPanel

## 
```c#
Implements ILoadingScreenPanel
```

## Summary

ImplementsILoadingScreenPanel.OnLoadingProgress
## Constructors

```c#
DefaultLoadingPanel( ) 
```
No Summary
## Fields

```c#
LoadingProgress Progress
```
No Summary
## Methods

```c#
virtual void OnLoadingProgress( LoadingProgress progress) 
```
ImplementsILoadingScreenPanel.OnLoadingProgress
```c#
protected override void BuildRenderTree( RenderTreeBuilder __builder) 
```
OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
```c#
protected override string GetRenderTreeChecksum( ) 
```
OverridesPanel.GetRenderTreeChecksumOverridden/implemented by Razor templating, contains render tree checksum to determine when the render tree content has changed.
