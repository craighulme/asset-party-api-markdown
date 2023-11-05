# MovementPathNodeEntity

## 
```c#
Derives from BasePathNodeEntity
```

## Summary

A movement path node.
## Constructors

```c#
MovementPathNodeEntity( ) 
```
No Summary
## Properties

```c#
EntityTarget AlternativeNodeBackwards { get; set; } 
```
Alternative node when moving backwards, for path changing.
```c#
EntityTarget AlternativeNodeForwards { get; set; } 
```
Alternative node when moving forwards, for path changing.
```c#
bool AlternativePathEnabled { get; set; } 
```
Whether the alternative path is enabled or not.
```c#
Output OnPassed { get; set; } 
```
Fired when an entity passes this node, depending on the entity implementation.
```c#
float Speed { get; set; } 
```
When passing this node, the moving entity will have its speed set to this value. 0 or less mean do not change.
## Methods

```c#
void DisablesAlternativePath( ) 
```
Disables the alternative path.
```c#
void EnableAlternativePath( ) 
```
Enables the alternative path.
```c#
void ToggleAlternativePath( ) 
```
Toggles the alternative path.
