# VROverlayPanel

## 
```c#
Derives from VROverlay
```

## Summary

ASandbox.VROverlaythat draws and handles input of aUI.RootPanel.VR overlays draw over the top of the 3D scene, they will not be affected by lighting,
post processing effects or anything else in the world.This makes them ideal for HUDs or menus, or anything else that should be local to the
HMD or tracked devices.If you need something in the world, consider using WorldPanel
andUI.WorldInputinstead.
## Constructors

```c#
VROverlayPanel( RootPanel panel) 
```
No Summary
## Properties

```c#
RootPanel RootPanel { get; init; } 
```
No Summary
## Methods

```c#
protected override void Dispose( bool disposing) 
```
OverridesVROverlay.Dispose
