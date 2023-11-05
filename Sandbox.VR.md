# VR

## Is static
Derives from object

## Summary

Gets or sets where the center of the VR play area is in world space.
By default this is yourGame.LocalPawntransform.
## Properties

```c#
static Transform Anchor { get; set; } 
```
Gets or sets where the center of the VR play area is in world space.
By default this is yourGame.LocalPawntransform.
```c#
static bool ControllersAreDrawing { get; } 
```
Returns true if SteamVR is drawing the controllers
```c#
static bool DashboardIsOpen { get; } 
```
Returns true if the SteamVR dashboard is visible
```c#
static bool Enabled { get; } 
```
Returns true if VR is active
```c#
static bool IsLeftHandDominant { get; } 
```
Returns true if the left hand is dominant
```c#
static float Scale { get; set; } 
```
Get or set the player's scale in the world. If you set it to 2 the player will be twice as big.
