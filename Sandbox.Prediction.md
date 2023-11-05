# Prediction

## 
```c#
Derives from object
```

## Summary

Client who is doing the predicting..
## Properties

```c#
static IClient CurrentHost { get; } 
```
Client who is doing the predicting..
```c#
static bool Enabled { get; } 
```
Whether prediction is currently enabled. SeePrediction.Off.
```c#
static bool FirstTime { get; } 
```
Returnstrueif this is the first time the client is trying to predict this event.
This is useful for one-time logic in your weapons (to prevent those events from being called rapidly in succession).
## Methods

```c#
static IDisposable Off( ) 
```
Temporarily disables prediction.Expected usage is like so:using ( Prediction.Off() )
 {
 	// Code that needs prediction disabled here...
 }
```c#
static bool WasPredicted( string name, object[] args) 
```
Used internally by ClientRPC system.
```c#
static void Watch( string name, object[] args) 
```
Used internally by ClientRPC system.
