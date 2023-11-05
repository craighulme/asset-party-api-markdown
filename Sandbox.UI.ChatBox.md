# ChatBox

## Derives from Panel

## Summary

OverridesPanel.TickCalled every frame. This is your "Think" function.
## Constructors

```c#
ChatBox( ) 
```
No Summary
## Properties

```c#
Panel Canvas { get; protected set; } 
```
No Summary
```c#
TextEntry Input { get; protected set; } 
```
No Summary
## Methods

```c#
static void AddChatEntry( string name, string message, string avatar = null, string lobbyState = null) 
```
No Summary
```c#
static void AddChatEntry( To to_target, string name, string message, string avatar = null, string lobbyState = null) 
```
No Summary
```c#
static void AddInformation( string message, string avatar = null) 
```
No Summary
```c#
static void AddInformation( To to_target, string message, string avatar = null) 
```
No Summary
```c#
static void Say( string message) 
```
No Summary
```c#
void AddEntry( string name, string message, string avatar, string lobbyState = null) 
```
No Summary
```c#
override void Tick( ) 
```
OverridesPanel.TickCalled every frame. This is your "Think" function.
