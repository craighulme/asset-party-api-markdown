# BindCollection

## Derives from object

## Summary

A collection of action binds.BindCollectionAction: attack1Slot0: mouse1Action: selectallSlot0: ctrl + aThe bind collection can be saved and loaded from disk via the BindSaveConfig class.The bind collection can have a base collection which it will fall back to if it contains
the same binds. This allows us to have a "common" collection which can be shared between
all games, but can also let the games + users to override those binds if they choose.
## Constructors

```c#
BindCollection( string name) 
```
Creates a collection and tries to load it from disk.
## Fields

```c#
CaseInsensitiveDictionary<ActionBind> Actions
```
The actual collection of binds.
## Properties

```c#
BindCollection Base { get; set; } 
```
The base collection. Game binds have this set to the common binds.
```c#
string CollectionName { get; set; } 
```
Will be either "common" or the ident of the current game.
```c#
string ConfigPath { get; set; } 
```
The location of the config file to load from in EngineFileSystem.Config
## Methods

```c#
string Get( string actionName, int slot) 
```
Get the bind value at this slot
```c#
ActionBind GetBind( string actionName, bool create = true) 
```
Get the bind, create if it doesn't exist
```c#
void SaveToDisk( ) 
```
Save the collection to disk
```c#
ActionBind Set( string actionName, int slot, string buttonName) 
```
Set the bind value for this action. This will overwrite what's in this slot.
## Nested Types

