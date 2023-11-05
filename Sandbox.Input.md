# Input

## 
```c#
Derives from object
```

## Summary

A client's current input state. On the client this always represents the input of the local player. On the server
this represents the input state of the client that is currently running their Simulate.
## Properties

```c#
static Angles AnalogLook { get; set; } 
```
Analog look value from the default input device.
```c#
static Vector3 AnalogMove { get; set; } 
```
Analog move value from the default input device.
```c#
static bool EscapePressed { get; } 
```
True if escape was pressed
```c#
static InputMotionData MotionData { get; } 
```
Current state of the current input device's motion sensor(s) if supported.
This is only supported on: Dualshock 4+, Switch Controllers, Steam Controller, Steam Deck.
```c#
static bool MouseCursorVisible { get; } 
```
True if the mouse cursor is visible (using UI etc)
```c#
static Vector2 MouseDelta { get; set; } 
```
Movement delta from the mouse.
```c#
static int MouseWheel { get; set; } 
```
The state of the mouse wheel.
```c#
static bool Paused { get; } 
```
Is the game currently paused?
```c#
static bool StopProcessing { get; set; } 
```
Should we stop processing input?
```c#
static bool UsingController { get; } 
```
If theSandbox.IClienthas used a controller input more recently then M+KB.
```c#
static bool UsingMouse { get; } 
```
If theSandbox.IClienthas used M+KB input more recently than a controller.
```c#
static VrInput VR { get; } 
```
Virtual Reality specific input data.
## Methods

```c#
static void Clear( string action) 
```
Remove this action, so it's no longer being pressed.
```c#
static void ClearActions( ) 
```
Clears the current input actions, so that none of them are active.
```c#
static void ClearButton( InputButton button) 
```
No Summary
```c#
static void ClearButtons( ) 
```
No Summary
```c#
static void CopyLastInput( IClient client) 
```
Copy the last input from the target client. This is useful for bots.
```c#
static bool Down( string action, bool complainOnMissing = true) 
```
Action is currently pressed down
```c#
static bool Down( InputButton button) 
```
No Summary
```c#
static Vector2 GetAnalog( InputAnalog axis) 
```
Returns a normalizedVector2of theSandbox.InputAnalogfrom the user's controller.
```c#
static string GetBindingForButton( string keyName) 
```
No Summary
```c#
static string GetButtonOrigin( string name, bool ignoreController = false) 
```
Returns the name of a key bound to this InputActionFor example:Input.GetButtonOrigin( "Undo" )could returnSPACEif using keyboard orA Buttonwhen using a controller.
```c#
static string GetButtonOrigin( InputAnalog analog) 
```
Returns the name of the analog axis bound to thisSandbox.InputAnalog.For example:Input.GetButtonOrigin( InputAnalog.Move )could returnLeft Joystick
```c#
static string GetButtonOrigin( InputButton button, bool ignoreController = false) 
```
No Summary
```c#
static Texture GetGlyph( string name, InputGlyphSize size = 0, GlyphStyle style = null) 
```
Get a glyph texture from the controller bound to the action.
If no binding is found will return an 'UNBOUND' glyph.
```c#
static Texture GetGlyph( InputAnalog analog, InputGlyphSize size = 0) 
```
Get a glyph texture from an analog input on a controller.
```c#
static Texture GetGlyph( InputButton button, InputGlyphSize size = 0, GlyphStyle style = null) 
```
No Summary
```c#
static string GetKeyWithBinding( string binding) 
```
No Summary
```c#
static bool Pressed( string action) 
```
Action wasn't pressed but now it is
```c#
static bool Pressed( InputButton button) 
```
No Summary
```c#
static void ReleaseAction( string name) 
```
Releases the action, and it won't be active again until it's pressed again. This really only works clientside.
```c#
static void ReleaseActions( ) 
```
Clears the current input actions, so that none of them are active. Unlike ClearActions
this will unpress the buttons, so they won't be active again until they're pressed again.
```c#
static bool Released( string action) 
```
Action was pressed but now it isn't
```c#
static bool Released( InputButton button) 
```
No Summary
```c#
static void SetAction( string action, bool down) 
```
Activates / Deactivates an action when building input.
```c#
static void SetButton( InputButton button, bool down = true) 
```
No Summary
```c#
static void SuppressButton( InputButton button) 
```
No Summary
## Nested Types

