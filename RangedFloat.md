# RangedFloat

## Derives from ValueType

## Summary

A float between two values, which can be randomized or fixed.
## Constructors

```c#
RangedFloat( float fixedValue) 
```
Initialize the float as a fixed value.
```c#
RangedFloat( float min, float max) 
```
Initialize the float as a random value between given min and max.
## Fields

```c#
float x
```
The minimum value of the float range.
```c#
float y
```
The maximum value of the float range.
## Properties

```c#
RangeType Range { get; set; } 
```
Range type of this float.
## Methods

```c#
static RangedFloat Parse( string str) 
```
Parse a ranged float from a string. Format is"min max rangetype".
```c#
float GetValue( ) 
```
Returns the final value of this ranged float, randomizing between min and max values.
```c#
override string ToString( ) 
```
OverridesValueType.ToString
## Operators

```c#
implicit RangedFloat =( float input) 
```
No Summary
## Nested Types

## Referencing Members

```c#
RangedFloat = DecalEntry.Depth { get; set; } 
```
```c#
RangedFloat = StingSound.Distance { get; set; } 
```
```c#
RangedFloat = DecalEntry.FadeDuration { get; set; } 
```
```c#
RangedFloat = DecalEntry.FadeTime { get; set; } 
```
```c#
RangedFloat = DecalEntry.Height { get; set; } 
```
```c#
RangedFloat = Soundscape.MasterVolume { get; set; } 
```
```c#
RangedFloat = SoundEvent.Pitch { get; set; } 
```
```c#
RangedFloat = StingSound.RepeatTime { get; set; } 
```
```c#
RangedFloat = DecalEntry.Rotation { get; set; } 
```
```c#
RangedFloat = RangedFloatProperty.Value { get; set; } 
```
```c#
RangedFloat = RangedFloatSliderProperty.Value { get; set; } 
```
```c#
RangedFloat = SoundEvent.Volume { get; set; } 
```
```c#
RangedFloat = LoopedSound.Volume { get; set; } 
```
```c#
RangedFloat = DecalEntry.Width { get; set; } 
```
