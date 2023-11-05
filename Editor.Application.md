# Application

## ```c#
Derives from object
```

## Summary

If true (default) then keyboard shortcuts will work. If false then shortcuts will be suppressed.
It's useful to suppress shortcuts when doing things like controlling a scene using WSAD etc.
## Properties

```c#
static bool AllowShortcuts { get; set; } 
```
If true (default) then keyboard shortcuts will work. If false then shortcuts will be suppressed.
It's useful to suppress shortcuts when doing things like controlling a scene using WSAD etc.
```c#
static Vector2 CursorDelta { get; } 
```
The cursor delta between this and previous frame.
```c#
static Vector2 CursorPosition { get; set; } 
```
Get/Set cursor position.
```c#
static float DpiScale { get; } 
```
No Summary
```c#
static KeyboardModifiers KeyboardModifiers { get; } 
```
Returns which keyboard modified keys are held down right at this point.
```c#
static MouseButtons MouseButtons { get; } 
```
Returns the current state of the mouse buttons.
```c#
static Vector2 UnscaledCursorPosition { get; set; } 
```
The cursor position, not scaled for DPI
## Methods

```c#
static bool IsKeyDown( KeyCode code) 
```
Returns the current state of the mouse buttons.
```c#
static string KeyCodeToString( KeyCode code) 
```
Converts an editor keycode to a string used by the game
Qt::Key -> WindowsVirtualKey -> ButtonCode_t -> string
```c#
static void SetStyle( string style) 
```
No Summary
```c#
static void SetStyles( string style) 
```
Directly set CSS style sheet(s) for this widget. Same format as a .css file.
```c#
static void Spin( ) 
```
Will process all of the UI events - allowing the UI to stay responsive during a blocking call.
