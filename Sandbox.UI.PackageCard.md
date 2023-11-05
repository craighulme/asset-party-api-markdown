# PackageCard

## ```c#
Derives from Panel
```

## Summary

Called when the icon part of the card is pressed
## Constructors

```c#
PackageCard( ) 
```
No Summary
## Properties

```c#
string BackgroundImage { get; } 
```
No Summary
```c#
bool Decorated { get; set; } 
```
No Summary
```c#
string HoverIcon { get; set; } 
```
No Summary
```c#
Action OnLaunch { get; set; } 
```
Called when the icon part of the card is pressed
```c#
Package Package { get; set; } 
```
No Summary
## Methods

```c#
string FormatHoursPlayed( ) 
```
No Summary
```c#
string UpdatedString( ) 
```
No Summary
```c#
void UpdateFaves( string ident, long value) 
```
No Summary
```c#
void UpdateUsers( string ident, long value) 
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
