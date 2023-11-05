# KeyEvent

## Derives from ValueType

## Summary

Information about aEditor.Widgets keyboard event.
## Properties

```c#
bool Accepted { get; set; } 
```
Whether this event should be propagated to parent widgets (false) or not (true).
```c#
bool HasAlt { get; } 
```
WhetherAltkey was being held down at the time of the event.
```c#
bool HasCtrl { get; } 
```
WhetherControlkey was being held down at the time of the event.
```c#
bool HasShift { get; } 
```
WhetherShiftkey was being held down at the time of the event.
```c#
KeyCode Key { get; set; } 
```
The key that triggered this event.
```c#
KeyboardModifiers KeyboardModifiers { get; set; } 
```
The keyboard modifier keys that were held down at the moment the event triggered.
```c#
uint NativeKeyCode { get; set; } 
```
OS specific key code that triggered this event.
```c#
string Text { get; set; } 
```
Text theKeyEvent.Keywould type in a text field.
## Referencing Members

```c#
protected override void EditorMainWindow.OnKeyPress( KeyEvent ) 
```
```c#
protected override void BaseScrollWidget.OnKeyPress( KeyEvent ) 
```
```c#
protected override void ComboBox.OnKeyPress( KeyEvent ) 
```
```c#
protected virtual void GraphicsItem.OnKeyPress( KeyEvent ) 
```
```c#
protected override void LineEdit.OnKeyPress( KeyEvent ) 
```
```c#
protected virtual void Widget.OnKeyPress( KeyEvent ) 
```
```c#
protected override void AssetBrowser.OnKeyPress( KeyEvent ) 
```
```c#
protected override void AssetList.OnKeyPress( KeyEvent ) 
```
```c#
protected override void AssetPicker.OnKeyPress( KeyEvent ) 
```
```c#
protected override void BaseItemWidget.OnKeyPress( KeyEvent ) 
```
```c#
protected override void KeyBind.OnKeyPress( KeyEvent ) 
```
```c#
virtual void TreeNode.OnKeyPress( KeyEvent ) 
```
```c#
protected override void WebWidget.OnKeyPress( KeyEvent ) 
```
```c#
protected override void GraphView.OnKeyPress( KeyEvent ) 
```
```c#
protected override void PhonemeItem.OnKeyPress( KeyEvent ) 
```
```c#
protected override void Handle.OnKeyPress( KeyEvent ) 
```
```c#
protected virtual void BaseItemWidget.OnKeyPressOnItem( KeyEvent, object ) 
```
```c#
protected override void TreeView.OnKeyPressOnItem( KeyEvent, object ) 
```
```c#
protected virtual void GraphicsItem.OnKeyRelease( KeyEvent ) 
```
```c#
protected virtual void Widget.OnKeyRelease( KeyEvent ) 
```
```c#
protected override void WebWidget.OnKeyRelease( KeyEvent ) 
```
```c#
protected override void GraphView.OnKeyRelease( KeyEvent ) 
```
```c#
void AutoComplete.OnParentKeyPress( KeyEvent ) 
```
