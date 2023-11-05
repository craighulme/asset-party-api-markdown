# To

## ```c#
Implements IEnumerable<IClient>
```

## Summary

A wrapper to define which clients to send network things to. This
aims to make code more readable by having the target argument in generated
functions be more obvious and visible.
## Properties

```c#
static To Everyone { get; } 
```
The same as To.Multiple( Client.All )
## Methods

```c#
static To Multiple( IEnumerable<IClient> clients) 
```
Send to multiple clients
```c#
static To Single( Entity pawn) 
```
Send to a single client (the client owner of this pawn)
```c#
static To Single( IClient client) 
```
Send to a single client
```c#
virtual IEnumerator<IClient> GetEnumerator( ) 
```
ImplementsIEnumerable`1.GetEnumerator
```c#
bool IsRecipient( IClient client) 
```
Is this client a target recipient?
```c#
void SendCommand( string command) 
```
Send a console command to clients references by this class.
## Referencing Members

```c#
static void ChatBox.AddChatEntry( To, string, string, string, string ) 
```
```c#
static void ChatBox.AddInformation( To, string, string ) 
```
```c#
static void Decal.Clear( To, bool, bool ) 
```
```c#
void Player.Deafen( To, float ) 
```
```c#
static Sound = Sound.FromEntity( To, string, Entity ) 
```
```c#
static Sound = Sound.FromEntity( To, string, Entity, string ) 
```
```c#
static Sound = Sound.FromScreen( To, string, float, float ) 
```
```c#
static Sound = Sound.FromWorld( To, string, Vector3 ) 
```
```c#
static void Decal.Move( To, Entity, Entity ) 
```
```c#
virtual void GameManager.OnKilledMessage( To, long, string, long, string, string ) 
```
```c#
static void Decal.Place( To, DecalDefinition, Entity, int, Vector3, Rotation, Color ) 
```
```c#
void NetWrite.SendRpc( To?, Entity ) 
```
```c#
void NetWrite.SendRpc2( To?, BaseNetworkable ) 
```
```c#
void PrecipitationEntity.SetActive( To, bool ) 
```
```c#
void PrecipitationEntity.SetParticleState( To, bool ) 
```
```c#
void PrecipitationEntity.SetParticleTimeScale( To, float ) 
```
```c#
Sound = Sound.SetPitch( To, float ) 
```
```c#
Sound = Sound.SetPosition( To, Vector3 ) 
```
```c#
Sound = Sound.SetRandomPitch( To, float, float ) 
```
```c#
Sound = Sound.SetVolume( To, float ) 
```
```c#
Sound = Sound.Stop( To ) 
```
```c#
protected void PostProcessingEntity.TurnOffEffect( To ) 
```
```c#
protected void PostProcessingEntity.TurnOnEffect( To ) 
```
```c#
void GradientFogEntity.UpdateFogState( To, bool ) 
```
