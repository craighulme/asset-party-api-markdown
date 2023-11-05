# AnimGraphDirectPlayback

## Is abstract
Derives from object

## Summary

For communicating with a Direct Playback Anim Node, which allows code to tell it to play a given sequence
## Constructors

```c#
protected AnimGraphDirectPlayback( ) 
```
No Summary
## Properties

```c#
abstract int AnimationCount { get; } 
```
Get the number of animations that can be used.
```c#
abstract IEnumerable<string> Animations { get; } 
```
Get the list of animations that can be used.
```c#
abstract float Duration { get; } 
```
The duration of the currently playing sequence (seconds)
```c#
abstract string Name { get; } 
```
Returns the currently playing sequence.
```c#
abstract float StartTime { set; } 
```
Set the time at which the currently playing sequence should have had a cycle of zero.
This will adjust the current cycle of the sequence to match.
```c#
abstract float Time { get; } 
```
The elapsed time of the currently playing animation sequence (seconds)
```c#
abstract float TimeNormalized { get; } 
```
Get the cycle of the currently playing sequence.  Will return 0 if no sequence is playing.
## Methods

```c#
abstract void Cancel( ) 
```
Stop playing the override sequence.
```c#
abstract void Play( string name) 
```
Play the given sequence until it ends, then blend back.
Calling this function with a new sequence while another one is playing will immediately start blending from the old one to the new one.
```c#
abstract void Play( string name, Vector3 target, float heading, float interpTime) 
```
Same as the other Play function, but also sets a target position and heading for the sequence.
Over interpTime seconds, the entity's root motion will be augmented to move it to target and rotate it to heading.
