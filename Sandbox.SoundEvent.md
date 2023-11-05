# SoundEvent

## Derives from GameResource

## Summary

A sound event. It can play a set of random sounds with optionally random settings such as volume and pitch.
## Constructors

```c#
SoundEvent( ) 
```
No Summary
```c#
SoundEvent( string soundName, float volume = 0.5) 
```
No Summary
## Properties

```c#
int Decibels { get; set; } 
```
How loud is this sound, affects how far away it can be heard
```c#
float MaximumDistance { get; } 
```
Calculated maximum distance this sound event would be audible at.
```c#
float MinimumDistance { get; } 
```
Calculated minimum distance this sound event would be audible at full volume.
```c#
RangedFloat Pitch { get; set; } 
```
The base pitch of the sound.
```c#
SoundSelectionMode SelectionMode { get; set; } 
```
Selection strategy to use when picking from multiple sounds.
```c#
List<string> Sounds { get; set; } 
```
A random sound from the list will be selected to be played.
```c#
bool UI { get; set; } 
```
Is this sound 2D?
```c#
RangedFloat Volume { get; set; } 
```
How loud the sound should be.
## Methods

```c#
void Create( ) 
```
Registers this sound event for usage.Resource.ResourceNamemust be not empty, and be unique.
```c#
protected override void PostLoad( ) 
```
OverridesGameResource.PostLoadCalled when the asset is first loaded from disk.
```c#
protected override void PostReload( ) 
```
OverridesGameResource.PostReloadCalled when the asset is recompiled/reloaded from disk.
## Nested Types

