# MouseEvent

## 
```c#
Derives from ValueType
```

## Summary

Information about aEditor.Widgets mouse event.
## Properties

```c#
bool Accepted { get; set; } 
```
Whether this event should be propagated to parent widgets (false) or not (true).
```c#
MouseButtons Button { get; } 
```
The mouse button that triggered the event.
```c#
MouseButtons ButtonState { get; } 
```
The current mouse button state.
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
bool IsDoubleClick { get; } 
```
Whether this mouse event was a double click.
```c#
KeyboardModifiers KeyboardModifiers { get; set; } 
```
The keyboard modifier keys that were held down at the moment the event triggered.
```c#
bool LeftMouseButton { get; } 
```
Whether the event was triggered by the left mouse button.
```c#
Vector2 LocalPosition { get; } 
```
Position of the mouse cursor relative to the widgets top left corner.
```c#
bool MiddleMouseButton { get; } 
```
Whether the event was triggered by the left mouse button.
```c#
bool RightMouseButton { get; } 
```
Whether the event was triggered by the left mouse button.
```c#
Vector2 ScreenPosition { get; } 
```
Absolute position of the mouse cursor on the screen.
```c#
Vector2 WindowPosition { get; } 
```
Position of the mouse cursor relative to the top left corner of the window the widget belongs to.
## Referencing Members

```c#
protected virtual void Widget.OnDoubleClick( MouseEvent ) 
```
```c#
protected override void ExpandGroup.OnDoubleClick( MouseEvent ) 
```
```c#
protected override void BoolControlWidget.OnDoubleClick( MouseEvent ) 
```
```c#
protected override void BaseItemWidget.OnDoubleClick( MouseEvent ) 
```
```c#
protected virtual void BaseItemWidget.OnItemContextMenu( VirtualWidget, MouseEvent ) 
```
```c#
protected override void TreeView.OnItemContextMenu( VirtualWidget, MouseEvent ) 
```
```c#
protected virtual bool = BaseItemWidget.OnItemPressed( VirtualWidget, MouseEvent ) 
```
```c#
protected override bool = TreeView.OnItemPressed( VirtualWidget, MouseEvent ) 
```
```c#
protected virtual void Widget.OnMouseClick( MouseEvent ) 
```
```c#
protected override void AssetProperty.OnMouseClick( MouseEvent ) 
```
```c#
protected override void ColorProperty.OnMouseClick( MouseEvent ) 
```
```c#
protected override void ResourceControlWidget.OnMouseClick( MouseEvent ) 
```
```c#
protected override void DecibelSliderProperty.OnMouseClick( MouseEvent ) 
```
```c#
protected override void ObjectProperty.OnMouseClick( MouseEvent ) 
```
```c#
protected override void ResourceProperty<T>.OnMouseClick( MouseEvent ) 
```
```c#
protected override void IconButton.OnMouseClick( MouseEvent ) 
```
```c#
protected override void KeyBind.OnMouseClick( MouseEvent ) 
```
```c#
protected override void ItemRow.OnMouseClick( MouseEvent ) 
```
```c#
protected override void ToggleSwitch.OnMouseClick( MouseEvent ) 
```
```c#
protected override void VideoWidget.OnMouseClick( MouseEvent ) 
```
```c#
protected override void VideoNativeWidget.OnMouseClick( MouseEvent ) 
```
```c#
protected override void GameScenePicker.OnMouseMove( MouseEvent ) 
```
```c#
protected virtual void Widget.OnMouseMove( MouseEvent ) 
```
```c#
protected override void SoundPreview.OnMouseMove( MouseEvent ) 
```
```c#
protected override void CurveEditorPopup.OnMouseMove( MouseEvent ) 
```
```c#
protected override void ColorProperty.OnMouseMove( MouseEvent ) 
```
```c#
protected override void FloatControlWidget.OnMouseMove( MouseEvent ) 
```
```c#
protected override void FloatingPointProperty<T>.OnMouseMove( MouseEvent ) 
```
```c#
protected override void FloatSlider.OnMouseMove( MouseEvent ) 
```
```c#
protected override void IntProperty.OnMouseMove( MouseEvent ) 
```
```c#
protected override void FloatRangeSlider.OnMouseMove( MouseEvent ) 
```
```c#
protected override void BaseItemWidget.OnMouseMove( MouseEvent ) 
```
```c#
protected override void WebWidget.OnMouseMove( MouseEvent ) 
```
```c#
protected override void GraphView.OnMouseMove( MouseEvent ) 
```
```c#
protected override void AssetPreviewWidget.OnMouseMove( MouseEvent ) 
```
```c#
protected override void EngineView.OnMousePress( MouseEvent ) 
```
```c#
protected virtual void Widget.OnMousePress( MouseEvent ) 
```
```c#
protected override void SoundPreview.OnMousePress( MouseEvent ) 
```
```c#
protected override void CurveEditorPopup.OnMousePress( MouseEvent ) 
```
```c#
protected override void Curve2DProperty.OnMousePress( MouseEvent ) 
```
```c#
protected override void AssetBrowser.OnMousePress( MouseEvent ) 
```
```c#
protected override void ExpandGroup.OnMousePress( MouseEvent ) 
```
```c#
protected override void Inspector.OnMousePress( MouseEvent ) 
```
```c#
protected override void NoticeWidget.OnMousePress( MouseEvent ) 
```
```c#
protected override void BoolControlWidget.OnMousePress( MouseEvent ) 
```
```c#
protected override void CurveControlWidget.OnMousePress( MouseEvent ) 
```
```c#
protected override void EnumControlWidget.OnMousePress( MouseEvent ) 
```
```c#
protected override void FloatControlWidget.OnMousePress( MouseEvent ) 
```
```c#
protected override void FlagsProperty<T>.OnMousePress( MouseEvent ) 
```
```c#
protected override void FloatingPointProperty<T>.OnMousePress( MouseEvent ) 
```
```c#
protected override void FloatSlider.OnMousePress( MouseEvent ) 
```
```c#
protected override void IntProperty.OnMousePress( MouseEvent ) 
```
```c#
protected override void ObjectProperty.OnMousePress( MouseEvent ) 
```
```c#
protected override void OrganisationProperty.OnMousePress( MouseEvent ) 
```
```c#
protected override void FloatRangeSlider.OnMousePress( MouseEvent ) 
```
```c#
protected override void BaseItemWidget.OnMousePress( MouseEvent ) 
```
```c#
protected override void ToolButton.OnMousePress( MouseEvent ) 
```
```c#
protected override void WebWidget.OnMousePress( MouseEvent ) 
```
```c#
protected override void GraphView.OnMousePress( MouseEvent ) 
```
```c#
protected override void AssetPreviewWidget.OnMousePress( MouseEvent ) 
```
```c#
protected override void Option.OnMousePress( MouseEvent ) 
```
```c#
protected override void TagEntry.OnMousePress( MouseEvent ) 
```
```c#
protected override void TagOption.OnMousePress( MouseEvent ) 
```
```c#
protected override void LayerName.OnMousePress( MouseEvent ) 
```
```c#
protected override void MatrixButton.OnMousePress( MouseEvent ) 
```
```c#
protected override void GameScenePicker.OnMouseReleased( MouseEvent ) 
```
```c#
protected virtual void Widget.OnMouseReleased( MouseEvent ) 
```
```c#
protected override void SoundPreview.OnMouseReleased( MouseEvent ) 
```
```c#
protected override void CurveEditorPopup.OnMouseReleased( MouseEvent ) 
```
```c#
protected override void ColorSwatchWidget.OnMouseReleased( MouseEvent ) 
```
```c#
protected override void FloatControlWidget.OnMouseReleased( MouseEvent ) 
```
```c#
protected override void GradientControlWidget.OnMouseReleased( MouseEvent ) 
```
```c#
protected override void FloatingPointProperty<T>.OnMouseReleased( MouseEvent ) 
```
```c#
protected override void BaseItemWidget.OnMouseReleased( MouseEvent ) 
```
```c#
protected override void KeyBind.OnMouseReleased( MouseEvent ) 
```
```c#
protected override void WebWidget.OnMouseReleased( MouseEvent ) 
```
```c#
protected override void GraphView.OnMouseReleased( MouseEvent ) 
```
```c#
protected override void Filter.OnMouseReleased( MouseEvent ) 
```
```c#
protected virtual void Widget.OnMouseRightClick( MouseEvent ) 
```
```c#
protected override void AssetInspector.OnMouseRightClick( MouseEvent ) 
```
