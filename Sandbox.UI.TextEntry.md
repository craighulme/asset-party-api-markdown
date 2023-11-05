# TextEntry

## 
```c#
Implements IInputControl
```

## Summary

AUI.Panelthat the user can enter text into.
## Constructors

```c#
TextEntry( ) 
```
No Summary
## Properties

```c#
bool AllowEmojiReplace { get; set; } 
```
Whether to allow automatic replacement of emoji codes with their actual unicode emoji characters. SeeUI.Emoji.
```c#
Func<string, object[]> AutoComplete { get; set; } 
```
If you hook a method up here we'll do autocomplete on it.
Return a list if strings for given string input.
```c#
Color CaretColor { get; set; } 
```
Color of the text cursor/caret, the blinking line at which newly typed characters are inserted.
```c#
int CaretPosition { get; set; } 
```
Position of the text cursor/caret within the text, at which newly typed characters are inserted.
```c#
string CharacterRegex { get; set; } 
```
If set, will block the input of any character that doesn't match. Will also setTextEntry.HasValidationErrorsaccordingly.
```c#
bool Disabled { get; set; } 
```
Is the text entry disabled?
If disabled, will add a "disabled" class and prevent focus.
```c#
bool HasValidationErrors { get; set; } 
```
ImplementsIInputControl.HasValidationErrorsIf true then this control has validation errors and the input shouldn't be accepted.
```c#
string HistoryCookie { get; set; } 
```
If set, the history of this text entry will be stored and restored using this key in the localGlobalGameNamespace.Cookie.
```c#
int HistoryMaxItems { get; set; } 
```
Maximum amount of itemsTextEntry.AddToHistorywill keep.
Oldest items will be discarded as new ones are added.
```c#
string Icon { get; set; } 
```
If set, will display amaterial iconat the end of the text entry.
```c#
IconPanel IconPanel { get; protected set; } 
```
TheUI.IconPanelthat displaysTextEntry.Icon
```c#
Label Label { get; init; } 
```
TheTextEntry.Labelthat contains the text of this text entry.
TODO PAINDAY: This should be protected or internal, no?
```c#
int? MaxLength { get; set; } 
```
If set, visually signals when the input text is longer than this value. Will also setTextEntry.HasValidationErrorsaccordingly.
```c#
float? MaxValue { get; set; } 
```
If we're numeric, this is the highest numeric value allowed
```c#
int? MinLength { get; set; } 
```
If set, visually signals when the input text is shorter than this value. Will also setTextEntry.HasValidationErrorsaccordingly.
```c#
float? MinValue { get; set; } 
```
If we're numeric, this is the lowest numeric value allowed
```c#
bool Multiline { get; set; } 
```
Makes it possible to enter new lines into the text entry. (By pressing the Enter key, which no longer acts as the submit key)
```c#
string NumberFormat { get; set; } 
```
Affects formatting of the text whenTextEntry.Numericis enabled. Accepts any format that is supported by System.Single.ToString(System.String).See examples here.
```c#
bool Numeric { get; set; } 
```
When set to true, ensures only numeric values can be typed. Also appliesTextEntry.FixNumericon text.
```c#
Action<string> OnTextEdited { get; set; } 
```
Called when the text of this text entry is changed.
```c#
string Placeholder { get; set; } 
```
Text to display when the text entry is empty. Typically a very short description of the expected contents or function of the text entry.
```c#
string Prefix { get; set; } 
```
If set, will display given text before the text entry box.
```c#
Label PrefixLabel { get; protected set; } 
```
TheTextEntry.Labelthat showsTextEntry.Prefixtext.
```c#
string StringRegex { get; set; } 
```
If set,TextEntry.HasValidationErrorswill return true if doesn't match regex.
```c#
string Suffix { get; set; } 
```
If set, will display given text after the text entry box.
```c#
Label SuffixLabel { get; protected set; } 
```
TheTextEntry.Labelthat showsTextEntry.Suffixtext.
```c#
string Text { get; set; } 
```
Access to the raw text in the text entry.
```c#
int TextLength { get; } 
```
Amount of characters in the text of the text entry. Not bytes.
```c#
string Value { get; set; } 
```
The value of the text entry. ReturnsTextEntry.Text, but does special logic when setting text.
```c#
override bool AcceptsImeInput { get; } 
```
OverridesPanel.AcceptsImeInputAllowIME inputwhen this is focused.
```c#
override bool HasContent { get; } 
```
OverridesPanel.HasContentIf true, callsPanel.DrawContent.
## Methods

```c#
protected virtual void AutoCompleteCancel( ) 
```
Auto complete was canceled, restore text to what it was before we started, and remove the auto complete popup.
```c#
protected virtual void AutoCompleteSelectionChanged( ) 
```
Auto complete selection has changed. Update the text entry text to that selected value.
```c#
virtual bool CanEnterCharacter( Char c) 
```
Called when a character is typed by the player.
```c#
virtual void DestroyAutoComplete( ) 
```
Close and delete the auto complete popup panel.
```c#
virtual string FixNumeric( ) 
```
Called to ensure theTextEntry.Textis absolutely in the correct format, in this case - a valid number format.
```c#
virtual void OnValueChanged( ) 
```
Called when the text entry's value changes.
```c#
void AddToHistory( string str) 
```
Add given string to the history of this text entry.
The history can be accessed by the player by pressing up and down arrows with an empty text entry.
```c#
void ClearHistory( ) 
```
Clear the input history that was previously added viaTextEntry.AddToHistory.
```c#
void UpdateAutoComplete( ) 
```
Open the auto complete popup with values fromTextEntry.AutoComplete.
Close the popup if we have no auto complete entries.
```c#
void UpdateAutoComplete( object[] options) 
```
Open the auto complete popup with given values.
```c#
void UpdateValidation( ) 
```
Update the validation state of this control.
```c#
override void DrawContent( ref RenderState state) 
```
OverridesPanel.DrawContentCalled whenPanel.HasContentis set totrueto custom draw the panels content.
```c#
override string GetClipboardValue( bool cut) 
```
OverridesPanel.GetClipboardValueIf we have a value that can be copied to the clipboard, return it here.
```c#
protected override void OnBlur( PanelEvent e) 
```
OverridesPanel.OnBlurCalled when this panel loses input focus.
```c#
override void OnButtonEvent( ButtonEvent e) 
```
OverridesPanel.OnButtonEventCalled when any button, mouse (except for mouse4/5) and keyboard, are pressed or depressed while hovering this panel.
```c#
override void OnButtonTyped( ButtonEvent e) 
```
OverridesPanel.OnButtonTypedCalled when any keyboard button has been typed (pressed) while this panel has input focus. (Panel.Focus)
```c#
protected override void OnDoubleClick( MousePanelEvent e) 
```
OverridesPanel.OnDoubleClickCalled when the player double clicks the panel with the left mouse button.
```c#
protected override void OnDragSelect( SelectionEvent e) 
```
OverridesPanel.OnDragSelectCalled when the player moves the mouse after "press and holding" (or dragging) the panel.
```c#
protected override void OnEvent( PanelEvent e) 
```
OverridesPanel.OnEventCalled when variousUI.PanelEvents happen. Handles event listeners and many standard events by default.
```c#
protected override void OnFocus( PanelEvent e) 
```
OverridesPanel.OnFocusCalled when this panel receives input focus.
```c#
override void OnKeyTyped( Char k) 
```
OverridesPanel.OnKeyTypedCalled when a printable character has been typed (pressed) while this panel has input focus. (Panel.Focus)
```c#
protected override void OnMouseDown( MousePanelEvent e) 
```
OverridesPanel.OnMouseDownCalled when the player presses down the left or right mouse buttons while hovering this panel.
```c#
protected override void OnMouseMove( MousePanelEvent e) 
```
OverridesPanel.OnMouseMoveCalled when the cursor moves while hovering this panel.
```c#
protected override void OnMouseUp( MousePanelEvent e) 
```
OverridesPanel.OnMouseUpCalled when the player releases left or right mouse button.
```c#
override void OnPaste( string text) 
```
OverridesPanel.OnPasteCalled when the user presses CTRL+V while this panel has input focus.
```c#
override void SetProperty( string name, string value) 
```
OverridesPanel.SetPropertySet a property on the panel, such as special properties (class,id,styleandvalue, etc.) and properties of the panel's C# class.
```c#
override void Tick( ) 
```
OverridesPanel.TickCalled every frame. This is your "Think" function.
