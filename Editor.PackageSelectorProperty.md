# PackageSelectorProperty

## ```c#
Derives from LineEdit
```

## Summary

Whether to allow selecting multiple packages.
## Constructors

```c#
PackageSelectorProperty( Widget parent) 
```
No Summary
## Properties

```c#
protected virtual bool AllowMultiple { get; } 
```
Whether to allow selecting multiple packages.
```c#
protected virtual Type PackageType { get; } 
```
No Summary
```c#
override string Value { get; set; } 
```
OverridesLineEdit.ValueAlias ofLineEdit.Text, except disallows setting text whenWidget.IsFocusedistrue.
## Methods

```c#
void OpenMenu( ) 
```
No Summary
```c#
protected override void OnBlur( FocusChangeReason reason) 
```
OverridesLineEdit.OnBlurCalled when the widget loses keyboard focus.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override void OnReturnPressed( ) 
```
OverridesLineEdit.OnReturnPressedCalled when the user presses the return (Enter) key.
