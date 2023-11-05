# GameCreateModalOptions

## Derives from ValueType

## Summary

If we want to save these settings, for easy recreation, we can do that here
## Constructors

```c#
GameCreateModalOptions( ) 
```
No Summary
## Fields

```c#
string Cookie
```
If we want to save these settings, for easy recreation, we can do that here
```c#
GameConfiguration Default
```
The default settings
```c#
string MapFilter
```
Allows filtering the map list. Some examples:"type:map sort:popular""type:map game:facepunch.platformer"
```c#
bool MapSelection
```
If true, we'll allow the user to select the map
```c#
int MaxPlayers
```
Maximum players allowed to be selected. If this matches MinPlayers, we won't show the maxplayers option
```c#
int MinPlayers
```
Minimum players allowed to be selected
```c#
string ModalTitle
```
Title to show at the top of the modal
```c#
Action<GameConfiguration> OnStartGame
```
Called when Start Game is pressed in the modal
## Referencing Members

```c#
abstract void IModalSystem.CreateGame( GameCreateModalOptions ) 
```
```c#
static void Overlay.ShowCreateGame( GameCreateModalOptions ) 
```
