# TabContainer

## 
```c#
Derives from Panel
```

## Summary

A container with tabs, allowing you to switch between different sheets.You can position the tabs by adding the class tabs-bottom, tabs-left, tabs-right (default is tabs top)
## Constructors

```c#
TabContainer( ) 
```
No Summary
## Fields

```c#
List<Tab> Tabs
```
Access to the pages on this control
## Properties

```c#
string ActiveTab { get; set; } 
```
The tab that is active
```c#
bool NoBody { set; } 
```
If true we will act as a tab bar and have no body.
```c#
Panel SheetContainer { get; protected set; } 
```
A control housing the sheets
```c#
string TabCookie { get; set; } 
```
If a cookie is set then the selected tab will be saved and restored.
```c#
Panel TabsContainer { get; protected set; } 
```
A control housing the tabs
## Methods

```c#
Tab AddTab( Panel panel, string tabName, string title, string icon = null) 
```
Add a tab to the sheet.
```c#
void SwitchTab( Tab tab, bool setCookie = true) 
```
Switch to a specific tab.
```c#
override void OnTemplateSlot( INode element, string slotName, Panel panel) 
```
OverridesPanel.OnTemplateSlotTODO: Obsolete this and instead maybe we have something like [PanelSlot( "slotname" )] that
is applied on properties. Then when we find a slot="slotname" we chase up the heirachy and set the property.
```c#
override void SetProperty( string name, string value) 
```
OverridesPanel.SetPropertySet a property on the panel, such as special properties (class,id,styleandvalue, etc.) and properties of the panel's C# class.
## Nested Types

