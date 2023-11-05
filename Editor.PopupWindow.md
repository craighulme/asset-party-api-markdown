# PopupWindow

## Derives from Dialog

## Summary

A simple popup window to quickly display a message, optionally with custom actions.
## Constructors

```c#
PopupWindow( string title, string text, string buttonTxt = "OK", IDictionary<string, Action> extraButtons = null) 
```
No Summary
## Methods

```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
