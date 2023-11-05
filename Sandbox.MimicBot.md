# MimicBot

## 
```c#
Derives from Bot
```

## Summary

A bot that mimics another player.
## Constructors

```c#
MimicBot( ) 
```
No Summary
```c#
MimicBot( string name) 
```
No Summary
## Properties

```c#
bool ForceCrouch { get; set; } 
```
Whether the bot should be forced to crouch?
```c#
IClient TargetClient { get; set; } 
```
The client this bot should mimic.
## Methods

```c#
override void BuildInput( ) 
```
OverridesBot.BuildInputCalled serverside each frame to build the bot's input data. You can use this to set what
buttons a bot is pressing, or where they should be looking, for example.
