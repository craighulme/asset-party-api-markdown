# Stats

## Is static
Derives from object

## Summary

Get the global stats for the calling package
## Properties

```c#
static GlobalStats Global { get; } 
```
Get the global stats for the calling package
```c#
static PlayerStats LocalPlayer { get; } 
```
Get the global stats for the calling package
## Methods

```c#
static void Flush( ) 
```
Send any pending stats to the backend. Don't wait for confirmation of ingestiom, fire and forget.
```c#
static Task FlushAndWaitAsync( CancellationToken token = null) 
```
Send any pending stats to the backend, will wait until they're available for query before finishing.
```c#
static Task FlushAsync( CancellationToken token = null) 
```
Send any pending stats to the backend. Don't wait for confirmation of ingestiom, fire and forget.
```c#
static GlobalStats GetGlobalStats( string packageIdent) 
```
Get the global stats for this package
```c#
static PlayerStats GetLocalPlayerStats( string packageIdent) 
```
Get the global stats for this package
```c#
static PlayerStats GetPlayerStats( string packageIdent, long steamid) 
```
Get the stats for this package
```c#
static void Increment( string name, double amount, string context = null, object data = null) 
```
No Summary
```c#
static void Increment( IClient client, string name, double amount, string context = null, object data = null) 
```
No Summary
```c#
static void SetValue( string name, double amount, string context = null, object data = null) 
```
No Summary
```c#
static void SetValue( IClient client, string name, double value, string context = null, object data = null) 
```
No Summary
## Nested Types

