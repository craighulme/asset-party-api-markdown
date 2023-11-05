# IClient

## ```c#
Inherits IEntity
```

## Summary

If this client is a bot.
## Properties

```c#
abstract bool IsBot { get; } 
```
If this client is a bot.
```c#
abstract bool IsFriend { get; } 
```
Whether the client is your friend or not
```c#
abstract bool IsListenServerHost { get; } 
```
Returns true if this client is the listen server host
```c#
abstract bool IsUsingVr { get; } 
```
Whether the client is using Virtual Reality or not.
```c#
abstract string Name { get; } 
```
The Steam name of this client.
```c#
abstract int PacketLoss { get; } 
```
This client's packet loss as a percentage (0-100)
```c#
abstract IEntity Pawn { get; set; } 
```
The entity this client is controlling, i.e. their physical representation in the game world.
```c#
abstract int Ping { get; } 
```
The time it takes for a network message to get to this client
```c#
abstract PvsConfig Pvs { get; } 
```
Potentially Visible Set. Use this to add new areas to the player's PVS. This is useful if you're
spectating another entity and want to be able to see what they see etc.
```c#
abstract long SteamId { get; } 
```
The SteamId of this client
```c#
abstract IVoice Voice { get; } 
```
Information regarding the client's voice activity.
## Methods

```c#
virtual void AddInt( string key, int value = 1) 
```
Convenience function, adds given number at given key viaIClient.SetInt.
```c#
abstract string GetClientData( string key, string defaultValue = null) 
```
Gets the convar value from a ClientData convar
```c#
abstract T GetClientData<T,>( string key, T defaultValue = null) 
```
Gets the convar value from a ClientData convar
```c#
virtual int GetInt( string key, int defaultValue = 0) 
```
Convenience function, returns previously set (viaIClient.SetInt) integer value at given key viaIClient.GetValue.
```c#
abstract T GetValue<T,>( string key, T defaultValue = null) 
```
Retrieves the arbitrary client info value at given key, set previously byIClient.SetValue.
```c#
abstract void Kick( ) 
```
Kick this client from the server.
```c#
abstract void SendCommandToClient( string command) 
```
Send a console command to this client to be run.
```c#
virtual void SetInt( string key, int value) 
```
Convenience function, sets an integer info at given key viaIClient.SetValue.
```c#
abstract void SetValue( string key, object value) 
```
Sets an arbitrary client info value at given key. The value will be networked to clients, so it should be a networkable type.
## Nested Types

