# DoorEntity

## 
```c#
Implements IUse
```

## Summary

A basic door entity that can move or rotate. It can be a model or a mesh entity.
The door will rotate around the model's origin. For Hammer meshes the mesh origin can be set via the Pivot Tool.
## Constructors

```c#
DoorEntity( ) 
```
No Summary
## Properties

```c#
bool Breakable { get; set; } 
```
If the door model supports break pieces and has prop_data with health, this option can be used to allow the door to break like a normal prop would.
```c#
string CloseSound { get; set; } 
```
Sound to play when the door starts to close.
```c#
float Distance { get; set; } 
```
Moving door: The amount, in inches, of the door to leave sticking out of the wall it recedes into when pressed. Negative values make the door recede even further into the wall.
Rotating door: The amount, in degrees, that the door should rotate when it's pressed.
```c#
Function Ease { get; set; } 
```
The easing function for both movement and rotation
TODO: Expose to hammer in a nice way
```c#
string FullyClosedSound { get; set; } 
```
Sound to play when the door reaches it's fully closed position.
```c#
string FullyOpenSound { get; set; } 
```
Sound to play when the door reaches it's fully open position.
```c#
float InitialPosition { get; set; } 
```
How far the door should be open on spawn where 0% = closed and 100% = fully open.
```c#
bool Locked { get; set; } 
```
Whether this door is locked or not.
```c#
string LockedSound { get; set; } 
```
Sound to play when the door is attempted to be opened, but is locked.
```c#
Angles MoveDir { get; set; } 
```
The direction the door will move, when it opens.
```c#
bool MoveDirIsLocal { get; set; } 
```
If checked, the movement direction angle is in local space and should be rotated by the entity's angles after spawning.
```c#
DoorMoveType MoveDirType { get; set; } 
```
Movement type of the door.
```c#
string MovingSound { get; set; } 
```
Sound to play while the door is moving. Typically this should be looping or very long.
```c#
protected Output OnBreak { get; set; } 
```
Fired when the entity gets destroyed.
```c#
protected Output OnClose { get; set; } 
```
Fired when the door starts to close. This can be called multiple times during a single "door closing"
```c#
protected Output OnDamaged { get; set; } 
```
Fired when the entity gets damaged, even if it is unbreakable.
```c#
protected Output OnFullyClosed { get; set; } 
```
Called when the door fully closes.
```c#
protected Output OnFullyOpen { get; set; } 
```
Called when the door fully opens.
```c#
protected Output OnLockedUse { get; set; } 
```
Fired when a player tries to open/close this door with +use, but it's locked
```c#
protected Output OnOpen { get; set; } 
```
Fired when the door starts to open. This can be called multiple times during a single "door opening"
```c#
bool OpenAwayFromPlayer { get; set; } 
```
If checked, rotating doors will try to open away from the activator
```c#
FGDCurve OpenCurve { get; set; } 
```
Used to override the open/close animation of moving and rotating doors. X axis (input, left to right) is the animation, Y axis (output, bottom to top) is how open the door is at that point in the animation.
```c#
string OpenSound { get; set; } 
```
Sound to play when the door starts to open.
```c#
EntityTarget OtherDoorsToOpen { get; set; } 
```
If set, opening this door will open all doors with given entity name. You can also simply name all doors the same for this to work.
```c#
Flags SpawnSettings { get; set; } 
```
Settings that are only applicable when the entity spawns
```c#
float Speed { get; set; } 
```
The speed at which the door moves.
```c#
DoorState State { get; protected set; } 
```
Which position the door is in.
```c#
float TimeBeforeReset { get; set; } 
```
Amount of time, in seconds, after the door has opened before it closes automatically. If the value is set to -1, the door never closes itself.
## Methods

```c#
virtual bool IsUsable( Entity user) 
```
ImplementsIUse.IsUsableDictates whether this entity is usable by given user.
```c#
virtual bool OnUse( Entity user) 
```
ImplementsIUse.OnUseCalled when the (probably) player has used this entity.
```c#
void Break( ) 
```
Causes this prop to break, regardless if it is actually breakable or not. (i.e. ignores health and whether the model has gibs)
```c#
void Close( Entity activator = null) 
```
Close the door. Obeys locked state.
```c#
void Lock( ) 
```
Locks the door so it cannot be opened or closed.
```c#
void Open( Entity activator = null) 
```
Open the door. Obeys locked state.
```c#
void Toggle( Entity activator = null) 
```
Toggle the open state of the door. Obeys locked state.
```c#
void Unlock( ) 
```
Unlocks the door.
```c#
protected override void OnAnimGraphCreated( ) 
```
OverridesAnimatedEntity.OnAnimGraphCreatedAn anim graph has been created for this entity. You will want to set up initial AnimGraph parameters here.
```c#
protected override void OnAnimGraphTag( string tag, AnimGraphTagEvent fireMode) 
```
OverridesAnimatedEntity.OnAnimGraphTagCalled when the anim graph of this entity has a tag change.
This will be called only for "Status" type tags.
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
```c#
override void OnKilled( ) 
```
OverridesEntity.OnKilledCalled (fromEntity.TakeDamageby default unless overridden) when there's no health left.
```c#
override void OnNewModel( Model model) 
```
OverridesModelEntity.OnNewModelCalled when the model of this entity has changed.
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

