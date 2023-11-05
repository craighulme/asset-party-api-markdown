# NavHostPanel

## Derives from Panel

## Summary

A panel that acts like a website. A single page is always visible
but it will cache other views that you visit, and allow forward/backward navigation.
## Constructors

```c#
NavHostPanel( ) 
```
No Summary
## Fields

```c#
protected List<HistoryItem> Cache
```
No Summary
```c#
string CurrentQuery
```
The query part of the url
## Properties

```c#
Panel CurrentPanel { get; } 
```
The currently visible panel
```c#
string CurrentUrl { get; } 
```
The Url we're currently viewing
```c#
string DefaultUrl { get; set; } 
```
The Url we should go to when one isn't set
```c#
Panel NavigatorCanvas { get; set; } 
```
The panel in which we should create our pages
## Methods

```c#
virtual bool GoBack( ) 
```
To back to the previous page. Return true on success.
```c#
virtual bool GoBackUntilNot( string wildcard) 
```
Keep pressing the back button until our url doesn't match the passed wildcard string
```c#
virtual bool GoForward( ) 
```
Go forward, return true on success
```c#
protected virtual void NotFound( string url) 
```
No Summary
```c#
void AddDestination( string url, Type type) 
```
Instead of finding pages by attributes, we can fill them in manually here
```c#
IEnumerable<ValueTuple<string, string>> ExtractProperties( string[] parts, string url) 
```
No Summary
```c#
void Navigate( string url, bool redirectToDefault = true) 
```
Navigate to the passed url
```c#
protected override void OnBack( PanelEvent e) 
```
OverridesPanel.OnBackCalled when the player presses the "Back" button while hovering this panel, which is typically "mouse 5", aka one of the mouse buttons on its side.
```c#
protected override void OnForward( PanelEvent e) 
```
OverridesPanel.OnForwardCalled when the player presses the "Forward" button while hovering this panel, which is typically "mouse 4", aka one of the mouse buttons on its side.
```c#
protected override void OnParametersSet( ) 
```
OverridesPanel.OnParametersSetCalled after initialization
```c#
override void OnTemplateSlot( INode element, string slotName, Panel panel) 
```
OverridesPanel.OnTemplateSlotThis sucks this sucks this sucks
```c#
override void SetProperty( string name, string value) 
```
OverridesPanel.SetPropertySet a property on the panel, such as special properties (class,id,styleandvalue, etc.) and properties of the panel's C# class.
## Inheriting Types

