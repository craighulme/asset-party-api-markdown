# AudioSystem

## 
```c#
Derives from object
```

## Summary

Play a sound event by name.
## Properties

```c#
float ReverbScale { get; set; } 
```
No Summary
```c#
float ReverbVolume { get; set; } 
```
No Summary
## Methods

```c#
SoundHandle Play( string eventName) 
```
Play a sound event by name.
```c#
SoundHandle Play( string eventName, IEntity sourceEntity) 
```
Play a sound event by name.
```c#
SoundHandle Play( SoundEvent soundEvent, IEntity sourceEntity = null) 
```
Play a sound event by name.
```c#
void PreloadSound( string eventName) 
```
Precaches sound files associated with given sound event by name.
This helps avoid stutters on first load of each sound file.
```c#
void SetEffect( string name, float value, float velocity = 10, float fadeOut = -1) 
```
No Summary
