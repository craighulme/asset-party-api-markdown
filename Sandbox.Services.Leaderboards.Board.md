# Board

## Derives from object

## Summary

The description of this board, which was set in the backend.
## Constructors

```c#
Board( string package, string name) 
```
No Summary
## Properties

```c#
string Description { get; set; } 
```
The description of this board, which was set in the backend.
```c#
string DisplayName { get; set; } 
```
The display name of this board, which was set in the backend.
```c#
Entry[] Entries { get; set; } 
```
The group of entries for this board. This is usually the entries that surround
the TargetSteamId.
```c#
string Group { get; set; } 
```
global, country, friends
```c#
int MaxEntries { get; set; } 
```
The maximum entries to respond with.
```c#
long TargetSteamId { get; set; } 
```
The steamid to get information about. If unset then this defaults to the current player.
```c#
string Title { get; } 
```
The group name of this board. For example, "Global" for global, "Friends" for friends.
```c#
long TotalEntries { get; } 
```
The total number of chart entries for this board.
```c#
string Unit { get; } 
```
The unit type chosen for this board
## Methods

```c#
Task Refresh( CancellationToken cancellation = null) 
```
No Summary
