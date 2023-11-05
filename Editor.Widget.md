# Widget

## ```c#
Derives from QObject
```

## Summary

A generic widget.
## Constructors

```c#
Widget( Widget parent, bool isDarkWindow = false) 
```
The default widget constructor
## Fields

```c#
Action MouseClick
```
Called when this widget is left clicked (on mouse release).
```c#
Action MouseLeftPress
```
Called when this widget is left clicked (on mouse press).
```c#
Action MouseMiddlePress
```
Called when this widget is clicked with the mouse wheel (on mouse press).
```c#
Action<Vector2> MouseMove
```
Called when the mouse cursor is moved while being over this widget.
```c#
Action MouseRelease
```
Called when mouse is released over this widget.
```c#
Action MouseRightClick
```
Called when this widget is right clicked (on mouse release).
```c#
Action MouseRightPress
```
Called when this widget is right clicked (on mouse press).
```c#
Func<bool> OnPaintOverride
```
Override the widget's paint process.Returntrueto prevent the default paint action, which is to callWidget.OnPaint.
## Properties

```c#
virtual CursorShape Cursor { get; set; } 
```
Cursor override for this widget.
```c#
virtual bool ProvidesDebugMode { get; } 
```
If true then this widget has a debug mode that can be activated
```c#
virtual bool ReadOnly { get; set; } 
```
Makes the widget read only. I.e. You can copy text of a text entry, but can't edit it.
Applies retroactively to all children.
```c#
virtual string WindowTitle { get; set; } 
```
No Summary
```c#
bool AcceptDrops { get; set; } 
```
Accept drag and dropping shit on us
```c#
IEnumerable<Widget> Children { get; } 
```
Child widgets of this widget.
```c#
Margin ContentMargins { get; set; } 
```
No Summary
```c#
Rect ContentRect { get; } 
```
No Summary
```c#
bool DebugModeEnabled { get; set; } 
```
Enable debug mode on this widget.
```c#
bool DeleteOnClose { get; set; } 
```
Delete this widget when close is pressed
```c#
float DpiScale { get; } 
```
The scale this widget is using (multiplying Size by this value gives the actual native size)
```c#
bool Enabled { get; set; } 
```
Makes the widget not interactable. This is also usually be reflected visually by the widget.
The widget will not process any keyboard or mouse inputs. Applies retroactively to all children.
```c#
float FixedHeight { set; } 
```
Shortcut, setsWidget.MinimumHeightandWidget.MaximumHeight
```c#
float FixedWidth { set; } 
```
Shortcut, setsWidget.MinimumWidthandWidget.MaximumWidth
```c#
FocusMode FocusMode { get; set; } 
```
Sets the focus mode for this widget. This determines both how it will get focus and whether it will receive keyboard input.
```c#
Widget FocusProxy { get; set; } 
```
No Summary
```c#
bool HasMaximizeButton { get; set; } 
```
No Summary
```c#
float Height { get; set; } 
```
Utility to interact with a widget's width - use Size where possible
```c#
bool IsActiveWindow { get; } 
```
No Summary
```c#
bool IsBeingDroppedOn { get; } 
```
Whether something is being dragged over this widget.
```c#
bool IsDraggable { get; set; } 
```
Whether this widget can be drag and dropped onto other widgets.
```c#
bool IsFocused { get; } 
```
Whether this widget has keyboard focus.
```c#
bool IsFramelessWindow { get; set; } 
```
No Summary
```c#
bool IsMaximized { get; } 
```
No Summary
```c#
bool IsMinimized { get; } 
```
No Summary
```c#
bool IsPopup { get; set; } 
```
No Summary
```c#
bool IsPressed { get; } 
```
Whether this widget is currently being pressed down or not.
```c#
bool IsTooltip { get; set; } 
```
No Summary
```c#
bool IsUnderMouse { get; } 
```
No Summary
```c#
bool IsWindow { get; set; } 
```
No Summary
```c#
Layout Layout { get; set; } 
```
The widget's internal layout, if any. Must be created via SetLayout or otherwise set beforehand.
```c#
Rect LocalRect { get; } 
```
This panel's rect at 0,0
```c#
float MaximumHeight { get; set; } 
```
This widgets height should never be larger than the given value.
```c#
Vector2 MaximumSize { get; set; } 
```
SetsWidget.MaximumWidthandWidget.MaximumHeightsimultaneously.
```c#
float MaximumWidth { get; set; } 
```
This widgets width should never be larger than the given value.
```c#
float MinimumHeight { get; set; } 
```
This widgets height should never be smaller than the given value.
```c#
Vector2 MinimumSize { get; set; } 
```
SetsWidget.MinimumWidthandWidget.MinimumHeightsimultaneously.
```c#
float MinimumWidth { get; set; } 
```
This widgets width should never be smaller than the given value.
```c#
bool MouseTracking { get; set; } 
```
No Summary
```c#
string Name { get; set; } 
```
Name of the widget, usually for debugging purposes.
```c#
bool NoSystemBackground { get; set; } 
```
No Summary
```c#
Widget Parent { get; set; } 
```
Parent widget. If non null, position of this widget will be relative to the parent widget. Certain events will also propagate to the parent widget if unhandled.
```c#
Vector2 Position { get; set; } 
```
Position of this widget, relative to its parent if it has one.
```c#
Rect ScreenGeometry { get; } 
```
Returns the geometry of the screen this widget is currently on.
```c#
Vector2 ScreenPosition { get; } 
```
Position of the widget relative to the monitor's top left corner.
```c#
Rect ScreenRect { get; } 
```
This panel's rect in screen coordinates
```c#
bool ShowWithoutActivating { get; set; } 
```
No Summary
```c#
Vector2 Size { get; set; } 
```
Size of this widget.
```c#
string StatusTip { get; set; } 
```
If set, hovering over this widget will set the text of aEditor.StatusBarof the window the widget belongs to.
```c#
string ToolTip { get; set; } 
```
If set, this text will be displayed after a certain delay of hovering this widget with the mouse cursor.
```c#
bool TranslucentBackground { get; set; } 
```
No Summary
```c#
bool TransparentForMouseEvents { get; set; } 
```
No Summary
```c#
bool Visible { get; set; } 
```
Whether this widget is visible or not.
```c#
float Width { get; set; } 
```
Utility to interact with a widget's width - use Size where possible
```c#
float WindowOpacity { get; set; } 
```
No Summary
## Methods

```c#
virtual void ChildValuesChanged( Widget source) 
```
No Summary
```c#
virtual void Close( ) 
```
If a window - will close
```c#
protected virtual void DoLayout( ) 
```
Called to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
protected virtual bool FocusNext( ) 
```
No Summary
```c#
protected virtual bool FocusPrevious( ) 
```
No Summary
```c#
virtual void Hide( ) 
```
Make this widget not visible.
```c#
protected virtual void OnBlur( FocusChangeReason reason) 
```
Called when the widget loses keyboard focus.
```c#
protected virtual bool OnClose( ) 
```
Called when a window is about to be closed.
```c#
protected virtual void OnClosed( ) 
```
Called when a window is closed.
```c#
protected virtual void OnContextMenu( ContextMenuEvent e) 
```
Called afterWidget.OnMouseRightClick, for the purposes of opening a context menu.
```c#
protected virtual void OnDoubleClick( MouseEvent e) 
```
Called when the widget was double clicked with any mouse button.
```c#
virtual void OnDragDrop( DragEvent ev) 
```
Something was dragged and dropped on this widget. Apply the data here, if its valid.RequiresWidget.AcceptDropsto function.
```c#
virtual void OnDragHover( DragEvent ev) 
```
Cursor with drag and drop data moved on this widget.RequiresWidget.AcceptDropsto function.
```c#
virtual void OnDragLeave( ) 
```
Cursor with drag and drop data left the bounds of this widget.RequiresWidget.AcceptDropsto function.
```c#
protected virtual void OnDragStart( ) 
```
Called when dragging.Widget.IsDraggableshould be true.
```c#
protected virtual void OnFocus( FocusChangeReason reason) 
```
Called when the widget gains keyboard focus.
```c#
protected virtual void OnKeyPress( KeyEvent e) 
```
A key has been pressed. Your widget needs keyboard focus for this to be called - see FocusMode.
```c#
protected virtual void OnKeyRelease( KeyEvent e) 
```
A key has been released.
```c#
protected virtual void OnMouseClick( MouseEvent e) 
```
Called when this widget is left clicked (on mouse release).
```c#
protected virtual void OnMouseEnter( ) 
```
Mouse cursor entered the bounds of this widget.
```c#
protected virtual void OnMouseLeave( ) 
```
Mouse cursor exited the bounds of this widget.
```c#
protected virtual void OnMouseMove( MouseEvent e) 
```
Called when the mouse cursor is moved while being over this widget.
```c#
protected virtual void OnMousePress( MouseEvent e) 
```
Called when mouse is pressed over this widget.
```c#
protected virtual void OnMouseReleased( MouseEvent e) 
```
Called when mouse is released over this widget.
```c#
protected virtual void OnMouseRightClick( MouseEvent e) 
```
Called when this widget is right clicked (on mouse release).
```c#
protected virtual void OnMoved( ) 
```
Called when the widget was moved.
```c#
protected virtual void OnPaint( ) 
```
Override to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected virtual void OnResize( ) 
```
Called when the widgets' size was changed.
```c#
protected virtual void OnVisibilityChanged( bool visible) 
```
Called when the visibility of this widget changes.
```c#
protected virtual void OnWheel( WheelEvent e) 
```
Mouse wheel was scrolled while the mouse cursor was over this widget.
```c#
virtual void SetWindowIcon( string name) 
```
No Summary
```c#
virtual void SetWindowIcon( Pixmap icon) 
```
No Summary
```c#
virtual void Show( ) 
```
Make this widget visible.
```c#
protected virtual void Signal( WidgetSignal signal) 
```
No Summary
```c#
protected virtual Vector2 SizeHint( ) 
```
Should return the size this widget really wants to be if it can its way. The default
is that you don't care - and just to return whatever the base value is.
```c#
virtual void Update( ) 
```
Tell this widget that shit changed and it needs to redraw
```c#
void AdjustSize( ) 
```
Adjusts the size of the widget to fit its contents.
```c#
void Blur( ) 
```
Clear keyboard focus from this widget.
```c#
void ClearContext( string key) 
```
Remove a context on this widget. This will NOT remove contexts set from parent objects.
```c#
void ConstrainTo( Rect parentRect) 
```
Reposition this widget to ensure it is within the given rectangle.
```c#
void ConstrainToScreen( ) 
```
Constrain this widget to the screen it's currently on.
```c#
void DestroyChildren( ) 
```
Destroys all child widgets of this widget.
```c#
void DisableWindowActivation( ) 
```
Calling this will set the WS_EX_NOACTIVATE flag on the window internally, which will stop
it taking focus away from other windows.
```c#
void Focus( bool activateWindow = true) 
```
No Summary
```c#
Vector2 FromScreen( Vector2 p) 
```
Transform coordinates relative to the monitors's top left corner, to coordinates relative to panel's top left corner.
```c#
T GetContext<T,>( string key, T defaultIfMissing = null) 
```
Find a context on this widget. If not found, look at the parent. If not found, look at the parent.
This is useful for passing information down to child widgets without any effort.
```c#
bool IsModal( ) 
```
Returns true if this is a modal window. This means it will appear on top of everything and block input to everything else.
```c#
void Lower( ) 
```
Lowers the widget to the bottom of the parent widget's stack.
After this call the widget will be visually behind (and therefore obscured by) any overlapping sibling widgets.
```c#
void MakeMaximized( ) 
```
No Summary
```c#
void MakeMinimized( ) 
```
No Summary
```c#
void MakeSignal( string name) 
```
No Summary
```c#
void MakeWindowed( ) 
```
No Summary
```c#
void PostKeyEvent( KeyCode key) 
```
No Summary
```c#
void Raise( ) 
```
Raises this widget to the top of the parent widget's stack.
After this call the widget will be visually in front of any overlapping sibling widgets.
```c#
void RestoreGeometry( string state) 
```
Restore position and size previously stored viaWidget.SaveGeometry.
```c#
string SaveGeometry( ) 
```
Serialize position and size of this widget to a string, which can then be passed toWidget.RestoreGeometry.
```c#
void SetContext( string key, object value) 
```
Set a context value on this widget. This context will be available to its children via FindContext.
```c#
void SetEffectOpacity( float f) 
```
No Summary
```c#
void SetModal( bool on, bool application = false) 
```
Set this window to be modal. This means it will appear on top of everything and block input to everything else.
```c#
void SetSizeMode( SizeMode horizontal, SizeMode vertical) 
```
No Summary
```c#
void SetStyles( string sheet) 
```
Directly set CSS style sheet(s) for this widget. Same format as a .css file.
```c#
void SetStylesheetFile( string filename) 
```
Set a file to load CSS for this widget from.
```c#
protected void SignalValuesChanged( ) 
```
When a value on this widget changed due to user input (ie, checking a box, editing a form)
this is called, which sends a signal up the parent widgets.
```c#
Vector2 ToScreen( Vector2 p) 
```
Transform coordinates relative to the panel's top left corner, to coordinates relative to monitors's top left corner.
## Events

```c#
OnChildValuesChanged( Widget obj) 
```
No Summary
```c#
VisibilityChanged( bool obj) 
```
Called when the visibility of this widget changes.
## Nested Types

## Inheriting Types

