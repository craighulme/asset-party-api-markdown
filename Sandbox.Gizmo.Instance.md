# Instance

## ```c#
Implements IDisposable
```

## Summary

Holds the backend state for a Gizmo scope. This allows us to have multiple different gizmo
states (for multiple views, multiple windows, game and editor) and push them as the current
active state whenever needed.
## Constructors

```c#
Instance( ) 
```
No Summary
## Fields

```c#
Inputs Input
```
Input state. Should be setup before push.
## Properties

```c#
string ControlMode { get; set; } 
```
The current control mode. This is generally implementation specific.
We tend to use "mouse" and "firstperson".
```c#
bool Debug { get; set; } 
```
If true, we'll draw some debug information
```c#
bool DebugHitboxes { get; set; } 
```
If true we'll enable hitbox debugging
```c#
Inputs PreviousInput { get; } 
```
The previous input state
```c#
SelectionSystem Selection { get; set; } 
```
This frame's created (or re-used) objects
```c#
SceneSettings Settings { get; } 
```
Some global settings accessible to the gizmos. Your implementation
generally lets your users set up  these things to their preference,
and the gizmos should try to obey them.
```c#
SceneWorld World { get; init; } 
```
The SceneWorld this instance is writing to. This world exists only for this instance.
You need to add this world to your camera for it to render (!)
## Methods

```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.DisposeDestroy this instance, clean up any created resources/scene objects, destroy the world.
```c#
T GetValue<T,>( string name) 
```
Generic storage for whatever you want to do.
You're responsible for not spamming into this and cleaning up after yourself.
```c#
IDisposable Push( ) 
```
Push this instance as the global Gizmo state. All Gizmo calls during this scope
will use this instance.
```c#
void SetValue<T,>( string name, T value) 
```
Generic storage for whatever you want to do.
You're responsible for not spamming into this and cleaning up after yourself.
```c#
void StompCursorPosition( Vector2 position) 
```
Set all of the state's cursor positions to this value. This stomps previous values
which will effectively clear any deltas. This should be used prior to starting a loop.
## Extensions

```c#
bool FirstPersonCamera( SceneCamera camera, Widget canvas) 
```
Helper to easily set up all of the inputs for this camera and widget. This is assuming
that the passed in widget is the render panel.
```c#
void UpdateInputs( SceneCamera camera, Widget canvas = null) 
```
Helper to easily set up all of the inputs for this camera and widget. This is assuming
that the passed in widget is the render panel.
