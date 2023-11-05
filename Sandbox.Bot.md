# Bot

## Derives from object
Implements IValid

## Summary

Create a bot. When you create one of these, a fake client will join the server and its input and behavior
can be controlled by overriding the BuildInput method serverside. Bots otherwise act like regular clients
and also have their own pawn.
## Constructors

```c#
Bot( ) 
```
Create a bot with a random name.
```c#
Bot( string name) 
```
Create a bot with given name.
## Properties

```c#
static IReadOnlyList<Bot> All { get; } 
```
Contains all bots on the server.
```c#
virtual bool IsValid { get; } 
```
ImplementsIValid.IsValidWhether this object is valid or not.
```c#
IClient Client { get; } 
```
The fake client that this bot represents.
## Methods

```c#
static void SetDefaultNames( List<string> names) 
```
Set a list of default bot names. Unless a bot is given a specific name, a name
will be chosen from this list until they have all been used. If all names have been
used already, a random name will be chosen from the list.
```c#
virtual void BuildInput( ) 
```
Called serverside each frame to build the bot's input data. You can use this to set what
buttons a bot is pressing, or where they should be looking, for example.
```c#
virtual void Tick( ) 
```
Called serverside for each tick that the bot exists in the server.
## Inheriting Types

