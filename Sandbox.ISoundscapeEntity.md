# ISoundscapeEntity

## Is interface

## Summary

Position of the soundscape entity, for determining which one is closer.
## Properties

```c#
abstract Vector3 Position { get; } 
```
Position of the soundscape entity, for determining which one is closer.
```c#
abstract string Soundscape { get; } 
```
The soundscape resource to play.
## Methods

```c#
abstract void DrawDebugOverlays( ) 
```
Called when debug overlay mode selected (in the editor) is "Soundscapes"
```c#
abstract bool TestPosition( Vector3 position) 
```
Called by the soundscape system to test if a client is within soundscape bounds.
