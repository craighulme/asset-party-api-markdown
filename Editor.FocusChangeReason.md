# FocusChangeReason

## 
```c#
Derives from Enum
```

## Summary

Describes why aEditor.Widgets' keyboard focus has changed viaWidget.OnFocusandWidget.OnBlurcallbacks.
## Fields

```c#
static FocusChangeReason ActiveWindow = 3
```
No Summary
```c#
static FocusChangeReason Backtab = 2
```
No Summary
```c#
static FocusChangeReason MenuBar = 6
```
No Summary
```c#
static FocusChangeReason Mouse = 0
```
No Summary
```c#
static FocusChangeReason None = 8
```
No Summary
```c#
static FocusChangeReason Other = 7
```
No Summary
```c#
static FocusChangeReason Popup = 4
```
No Summary
```c#
static FocusChangeReason Shortcut = 5
```
No Summary
```c#
static FocusChangeReason Tab = 1
```
No Summary
## Referencing Members

```c#
protected override void ComboBox.OnBlur( FocusChangeReason ) 
```
```c#
protected override void LineEdit.OnBlur( FocusChangeReason ) 
```
```c#
protected virtual void Widget.OnBlur( FocusChangeReason ) 
```
```c#
protected override void Window.OnBlur( FocusChangeReason ) 
```
```c#
protected override void PackageSelectorProperty.OnBlur( FocusChangeReason ) 
```
```c#
protected override void WebWidget.OnBlur( FocusChangeReason ) 
```
```c#
protected override void LineEdit.OnFocus( FocusChangeReason ) 
```
```c#
protected virtual void Widget.OnFocus( FocusChangeReason ) 
```
```c#
protected override void WebWidget.OnFocus( FocusChangeReason ) 
```
