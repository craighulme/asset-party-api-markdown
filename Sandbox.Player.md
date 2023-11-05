# Player

## 
```c#
Derives from AnimatedEntity
```

## Summary

The PlayerController takes player input and moves the player. This needs
to match between client and server. The client moves the local player and
then checks that when the server moves the player, everything is the same.
This is called prediction. If it doesn't match the player resets everything
to what the server did, that's a prediction error.
You should really never manually set this on the client - it's replicated so
that setting the class on the server will automatically network and set it
on the client.
## Constructors

```c#
Player( ) 
```
No Summary
## Properties

```c#
Entity ActiveChild { get; set; } 
```
No Summary
```c#
Entity ActiveChildInput { get; set; } 
```
No Summary
```c#
PawnController Controller { get; set; } 
```
The PlayerController takes player input and moves the player. This needs
to match between client and server. The client moves the local player and
then checks that when the server moves the player, everything is the same.
This is called prediction. If it doesn't match the player resets everything
to what the server did, that's a prediction error.
You should really never manually set this on the client - it's replicated so
that setting the class on the server will automatically network and set it
on the client.
```c#
ModelEntity Corpse { get; set; } 
```
A generic corpse entity
```c#
PawnController DevController { get; set; } 
```
This is used for noclip mode
```c#
Vector3 EyeLocalPosition { get; set; } 
```
Position a player should be looking from in local to the entity coordinates.
```c#
Rotation EyeLocalRotation { get; set; } 
```
Rotation of the entity's "eyes", i.e. rotation for the camera when this entity is used as the view entity. In local to the entity coordinates.
```c#
Vector3 EyePosition { get; set; } 
```
Position a player should be looking from in world space.
```c#
Rotation EyeRotation { get; set; } 
```
Rotation of the entity's "eyes", i.e. rotation for the camera when this entity is used as the view entity.
```c#
Vector3 InputDirection { get; protected set; } 
```
No Summary
```c#
IBaseInventory Inventory { get; protected set; } 
```
Player's inventory for entities that can be carried. SeeSandbox.BaseCarriable.
```c#
Angles OriginalViewAngles { get; } 
```
No Summary
```c#
Entity Using { get; protected set; } 
```
Entity the player is currently using via their interaction key.
```c#
Angles ViewAngles { get; set; } 
```
No Summary
```c#
override Ray AimRay { get; } 
```
OverridesEntity.AimRayOverride the aim ray to use the player's eye position and rotation.
## Methods

```c#
virtual void CreateHull( ) 
```
Create a physics hull for this player. The hull stops physics objects and players passing through
the player. It's basically a big solid box. It also what hits triggers and stuff.
The player doesn't use this hull for its movement size.
```c#
protected virtual Entity FindUsable( ) 
```
Find a usable entity for this player to use
```c#
virtual float FootstepVolume( ) 
```
Allows override of footstep sound volume.
```c#
virtual PawnController GetActiveController( ) 
```
Return the controller to use. Remember any logic you use here needs to match
on both client and server. This is called as an accessor every tick.. so maybe
avoid creating new classes here or you're gonna be making a ton of garbage!
```c#
virtual void OnActiveChildChanged( Entity previous, Entity next) 
```
Called when the Active child is detected to have changed
```c#
virtual void Respawn( ) 
```
Sets LifeState to Alive, Health to Max, nulls velocity, and calls Gamemode.PlayerRespawn
```c#
virtual void SimulateActiveChild( IClient cl, Entity child) 
```
Simulated the active child. This is important because it calls ActiveEnd and ActiveStart.
If you don't call these things, viewmodels and stuff won't work, because the entity won't
know it's become the active entity.
```c#
protected virtual void StopUsing( ) 
```
If we're using an entity, stop using it
```c#
protected virtual void TickPlayerUse( ) 
```
This should be called somewhere in your player's tick to allow them to use entities
```c#
protected virtual void UseFail( ) 
```
Player tried to use something but there was nothing there.
Tradition is to give a disappointed boop.
```c#
void Deafen( float strength) 
```
Applies flashbang-like ear ringing effect to the player.
```c#
void Deafen( To toTarget, float strength) 
```
Applies flashbang-like ear ringing effect to the player.
```c#
protected bool IsValidUseEntity( Entity e) 
```
Returns if the entity is a valid usable entity
```c#
override void BuildInput( ) 
```
OverridesEntity.BuildInputCalled from the gamemode, clientside only.
```c#
override void FrameSimulate( IClient cl) 
```
OverridesEntity.FrameSimulateCalled each frame clientside only on Pawn (and anything the pawn decides to call it on).
```c#
override void OnAnimEventFootstep( Vector3 pos, int foot, float volume) 
```
OverridesModelEntity.OnAnimEventFootstepA footstep has arrived!
```c#
override void OnChildAdded( Entity child) 
```
OverridesEntity.OnChildAddedCalled when an entity is parented to this entity.
```c#
override void OnChildRemoved( Entity child) 
```
OverridesEntity.OnChildRemovedCalled when an entity is unparented from this entity.
```c#
override void OnKilled( ) 
```
OverridesEntity.OnKilledCalled once the player's health reaches 0.
```c#
override void Simulate( IClient cl) 
```
OverridesEntity.SimulateCalled every tick to simulate the player. This is called on the
client as well as the server (for prediction). So be careful!
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
```c#
override void StartTouch( Entity other) 
```
OverridesEntity.StartTouchAn entity has started touching this trigger entity. RequiresEnableTouchenabled on this entity.For solid collisions, seeEntity.OnPhysicsCollision.
```c#
override void TakeDamage( DamageInfo info) 
```
OverridesEntity.TakeDamageCalled when the entity receives a damage event. This is where you want to subtract health, etc.
