# Scoreboard<T>

## 
```c#
Derives from Panel
```

## Summary

OverridesPanel.TickCalled every frame. This is your "Think" function.
## Type Parameters

```c#
T is ScoreboardEntry, new(), 
```
No Summary
## Constructors

```c#
Scoreboard( ) 
```
No Summary
## Properties

```c#
Panel Canvas { get; protected set; } 
```
No Summary
```c#
Panel Header { get; protected set; } 
```
No Summary
## Methods

```c#
protected virtual T AddClient( IClient entry) 
```
No Summary
```c#
protected virtual void AddHeader( ) 
```
No Summary
```c#
virtual bool ShouldBeOpen( ) 
```
No Summary
```c#
override void Tick( ) 
```
OverridesPanel.TickCalled every frame. This is your "Think" function.
