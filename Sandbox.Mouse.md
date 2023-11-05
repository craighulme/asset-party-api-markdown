# Mouse

## 
```c#
Derives from object
```

## Summary

Whether the local clients' cursor is active or not, meaning it can interact with UI elements, etc.
## Properties

```c#
static bool Active { get; } 
```
Whether the local clients' cursor is active or not, meaning it can interact with UI elements, etc.
```c#
static string CursorType { get; set; } 
```
Sets the cursor type until another panel stomps this value.
Doesn't affect main menu.
```c#
static Vector2 Delta { get; } 
```
Change in local clients' cursor position since last frame.
```c#
static Vector2 Position { get; set; } 
```
Access to local clients' cursor position, relative to game windows' top left corner.
```c#
static Vector2 Velocity { get; } 
```
No Summary
```c#
static bool Visible { get; } 
```
Whether the local clients' cursor is visible or not.
