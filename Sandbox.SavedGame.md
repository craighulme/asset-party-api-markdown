# SavedGame

## Derives from object

## Summary

Holds metadata and raw data relating to a Saved Game.
## Constructors

```c#
SavedGame( ) 
```
No Summary
## Properties

```c#
byte[] Data { get; set; } 
```
Serialized byte array representing the raw data for this Saved Game.
```c#
string Map { get; set; } 
```
The full ident of the map. This will default to the current map if it isn't set.
```c#
Metadata Metadata { get; } 
```
Any metadata associated with this Saved Game.
```c#
string Name { get; set; } 
```
The display name of the Saved Game.
```c#
DateTime Time { get; } 
```
Get the time when this Saved Game was last saved.
```c#
int Version { get; } 
```
The format version for this Saved Game.
## Methods

```c#
string GetDataAsString( ) 
```
Get the raw data as a string. This could be serialized JSON.
```c#
void SetData( string data) 
```
Set the raw data as a string. This could be serialized JSON.
