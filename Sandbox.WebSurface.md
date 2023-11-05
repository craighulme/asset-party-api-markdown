# WebSurface

## ```c#
Implements IDisposable
```

## Summary

Enables rendering and interacting with a webpage
## Properties

```c#
string Cursor { get; } 
```
No Summary
```c#
bool HasKeyFocus { get; set; } 
```
Tell the html control if it has key focus currently, controls showing the I-beam cursor in text controls amongst other things
```c#
bool InBackgroundMode { get; set; } 
```
Enable/disable low-resource background mode, where javascript and repaint timers are throttled, resources are
more aggressively purged from memory, and audio/video elements are paused. When background mode is enabled,
all HTML5 video and audio objects will execute ".pause()" and gain the property "._steam_background_paused = 1".
When background mode is disabled, any video or audio objects with that property will resume with ".play()".
```c#
bool IsLimited { get; } 
```
No Summary
```c#
TextureChangedDelegate OnTexture { get; set; } 
```
Called when the texture has changed and should be updated
```c#
string PageTitle { get; } 
```
No Summary
```c#
float ScaleFactor { get; set; } 
```
DPI Scaling factor
```c#
Vector2 Size { get; set; } 
```
The size of the browser
```c#
string Url { get; set; } 
```
The current Url
## Methods

```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.Dispose
```c#
void TellChar( uint unicodeKey, KeyboardModifiers modifiers) 
```
Tell the browser a unicode key has been pressed
```c#
void TellKey( uint virtualKeyCode, KeyboardModifiers modifiers, bool state) 
```
Tell the browser a key has been pressed or released
```c#
void TellMouseButton( MouseButtons button, bool state) 
```
Tell the browser a mouse button has been pressed
```c#
void TellMouseMove( Vector2 position) 
```
Tell the browser the mouse has moved
```c#
void TellMouseWheel( int delta) 
```
Tell the browser the mouse wheel has moved
## Nested Types

