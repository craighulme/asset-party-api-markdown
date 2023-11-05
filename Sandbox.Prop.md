# Prop

## 
```c#
Derives from BasePhysics
```

## Summary

A prop that physically simulates as a single rigid body. It can be constrained to other physics objects using hinges
or other constraints. It can also be configured to break when it takes enough damage.
Note that the health of the object will be overridden by the health inside the model, to ensure consistent health game-wide.
If the model used by the prop is configured to be used as a prop_dynamic (i.e. it should not be physically simulated) then it CANNOT be
used as a prop_physics. Upon level load it will display a warning in the console and remove itself. Use a prop_dynamic instead.
## Constructors

```c#
Prop( ) 
```
No Summary
## Properties

```c#
RealTimeUntil Invulnerable { get; set; } 
```
This prop won't be able to be damaged for this amount of time
```c#
protected Output OnBreak { get; set; } 
```
Fired when the entity gets destroyed.
```c#
protected Output OnDamaged { get; set; } 
```
Fired when the entity gets damaged.
```c#
bool Static { get; set; } 
```
If set, the prop will spawn with motion disabled and will act as a navigation blocker until broken.
## Methods

```c#
protected virtual void UpdatePropData( Model model) 
```
Called on new model to update the prop withNodes.ModelPropDatadata of the new model.
```c#
void Break( ) 
```
Causes this prop to break, regardless if it is actually breakable or not. (i.e. ignores health and whether the model has gibs)
```c#
protected void DeleteInput( ) 
```
Deletes this prop.
```c#
Task ExplodeAsync( float fTime) 
```
TODO: Internal, explodes and spawns gibs
```c#
protected void SetBodyGroupInput( string group) 
```
Sets the body group of the props' model by name, as set in ModelDoc.
Format is "name,option"
```c#
protected void SetCollisions( bool enabled) 
```
Enables or disables collisions on this prop.
```c#
protected void SetMaterialGroupInput( string group) 
```
Sets the material group of the props' model by name, as set in ModelDoc.
```c#
protected void SetScale( float scale) 
```
Sets the scale of the prop, affecting physics and visual scale.
```c#
protected void SetStatic( bool enabled) 
```
Enables or disables physics (gravity) simulation of this prop.
```c#
protected void SetVisible( bool enabled) 
```
Enables or disables visibility of this prop.
```c#
void Unweld( bool reweldChildren = false, Prop reweldProp = null) 
```
Unweld this prop from other props.
```c#
void Weld( Prop prop) 
```
Weld this prop to the given prop. This will merge their physics shapes with this prop's shapes.
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
protected override void OnPhysicsCollision( CollisionEventData eventData) 
```
OverridesBasePhysics.OnPhysicsCollisionCalled when this entity collides with anything else via Physics.
```c#
override void Spawn( ) 
```
OverridesBasePhysics.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
```c#
override void TakeDamage( DamageInfo info) 
```
OverridesBasePhysics.TakeDamageCalled when the entity receives a damage event. This is where you want to subtract health, etc.
## Inheriting Types

