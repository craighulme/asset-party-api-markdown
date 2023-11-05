# ButtonEntity

## Derives from KeyframeEntity
Implements IUse

## Summary

A generic button that is useful to control other map entities via inputs/outputs.
## Constructors

```c#
ButtonEntity( ) 
```
No Summary
## Properties

```c#
ActivationFlags ActivationSettings { get; set; } 
```
How this button can be activated
```c#
float Distance { get; set; } 
```
Moving button: The amount, in inches, of the button to leave sticking out of the wall it recedes into when pressed. Negative values make the button recede even further into the wall.
Rotating button: The amount, in degrees, that the button should rotate when it's pressed.
```c#
bool Locked { get; set; } 
```
Whether the button is locked or not.
```c#
string LockedSound { get; set; } 
```
Sound played when the button is pressed and is locked
```c#
bool Momentary { get; set; } 
```
If enabled, the button will have to be held to reach the pressed in state.
```c#
Angles MoveDir { get; set; } 
```
Specifies the direction to move in when the button is used, or axis of rotation for rotating buttons.
```c#
bool MoveDirIsLocal { get; set; } 
```
If checked, the movement direction angle is in local space and should be rotated by the entity's angles after spawning.
```c#
ButtonMoveType MoveDirType { get; set; } 
```
Movement type of the button.
```c#
protected Output OnDamaged { get; set; } 
```
Fired when the button is damaged
```c#
protected Output OnIn { get; set; } 
```
Fired when the button reaches the in/pressed position
```c#
protected Output OnOut { get; set; } 
```
Fired when the button reaches the out/released position
```c#
protected Output OnPressed { get; set; } 
```
Fired when the button is pressed by any means. This is not the same as button reaching its pressed in position.
```c#
protected Output<float> OnProgress { get; set; } 
```
Fired when the button position changes, carries 0...1 as argument.
```c#
protected Output OnReleased { get; set; } 
```
Fired when the button was released. This is not the same as button reaching its initial position.
```c#
protected Output OnUseLocked { get; set; } 
```
Fired when the button is used while locked
```c#
float Progress { get; protected set; } 
```
Represents the button's position between being fully pressed (1) and fully depressed (0). Used forButtonEntity.OnProgressHammer output.
```c#
float ResetDelay { get; set; } 
```
Amount of time, in seconds, after the button has been fully pressed before it starts to return to the starting position. Once it has returned, it can be used again. If the value is set to -1, the button never returns.
```c#
float ReturnSpeed { get; set; } 
```
The speed at which the button returns to the initial position. 0 or less will function as the 'forward' move speed.
```c#
Flags SpawnSettings { get; set; } 
```
Settings that are only relevant on spawn
```c#
float Speed { get; set; } 
```
The speed at which the button moves, in inches per second or degrees per second.
```c#
bool Toggle { get; set; } 
```
If enabled, the button will have to be activated again to return to initial position.
```c#
string UnlockedSound { get; set; } 
```
Sound played when the button is pressed and is unlocked
## Methods

```c#
virtual bool IsUsable( Entity user) 
```
ImplementsIUse.IsUsableDictates whether this entity is usable by given user.
```c#
virtual bool OnUse( Entity user) 
```
ImplementsIUse.OnUseA player has pressed this
```c#
protected void Lock( ) 
```
Become locked
```c#
protected void Press( Entity activator) 
```
Simulates the button being pressed
```c#
protected void Unlock( ) 
```
Become unlocked
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
```c#
override void TakeDamage( DamageInfo info) 
```
OverridesEntity.TakeDamageCalled when the entity receives a damage event. This is where you want to subtract health, etc.
## Nested Types

