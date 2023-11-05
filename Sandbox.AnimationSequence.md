# AnimationSequence

## Is abstract
Derives from object

## Summary

The duration of the currently playing sequence (seconds)
## Constructors

```c#
protected AnimationSequence( ) 
```
No Summary
## Properties

```c#
abstract float Duration { get; } 
```
The duration of the currently playing sequence (seconds)
```c#
abstract bool IsFinished { get; } 
```
Get whether the current animation sequence has finished
```c#
abstract string Name { get; set; } 
```
The name of the currently playing animation sequence
```c#
abstract float Time { get; set; } 
```
The elapsed time of the currently playing animation sequence (seconds)
```c#
abstract float TimeNormalized { get; set; } 
```
The normalized (between 0 and 1) elapsed time of the currently playing
animation sequence
