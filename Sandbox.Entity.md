# Entity

## 
```c#
Implements IEntity
```

## Summary

A base entity all other entities derive from.
## Constructors

```c#
Entity( ) 
```
Create the entity.
## Fields

```c#
readonly EntityTags Tags
```
Accessor to add, remove and check entity tags
```c#
TaskSource Task
```
Allows System.Threading.Tasks.Task.Delay(System.Int32) and similar calls that are automatically canceled when the entity is destroyed
## Properties

```c#
static IReadOnlyList<Entity> All { get; } 
```
A list of all active entities.
```c#
static bool AutoFlushSpawn { get; set; } 
```
Auto call TryAutoFlushSpawn() after creating an entity, so it's
spawned straight away. This is kept internal on purpose. We need
to consider a lot of things before letting people control this.
```c#
virtual Ray AimRay { get; } 
```
ImplementsIEntity.AimRayGet a ray representing where this entity is aiming. This can differ from the entity's
position and rotation, for example in a first person shooter the player's body is usually
aiming in different direction to the player's eyes.
```c#
virtual Angles AngularVelocity { get; set; } 
```
The angular velocity in local coordinates.
```c#
virtual IClient Client { get; } 
```
ImplementsIEntity.ClientThe client that owns this entity. Usually as a result of being the client's Pawn.
Also could be because the client's pawn owns this entity,
```c#
virtual IComponentSystem Components { get; } 
```
ImplementsIEntity.ComponentsComponents of this entity.
```c#
virtual string HammerID { get; set; } 
```
Unique ID for entities spawned by map.
```c#
virtual bool IsAuthority { get; } 
```
ImplementsIEntity.IsAuthorityReturns true if we have authority over this entity. This means we're either serverside,
or we're a clientside entity, or we're a serverside entity being predicted on the client.
```c#
virtual bool IsClientOnly { get; } 
```
ImplementsIEntity.IsClientOnlyTrue if this entity is a purely clientside entity, with no serverside components
```c#
virtual bool IsDormant { get; } 
```
ImplementsIEntity.IsDormantReturns true if this entity is dormant (the client cannot see it, it isn't being networked)
```c#
virtual bool IsFirstPersonMode { get; } 
```
If this entity is being viewed through, or is a child of an entity that is being view
through - will return true. This can be read are we in first person mode.
```c#
virtual bool IsFromMap { get; } 
```
ImplementsIEntity.IsFromMapReturns true if this specific entity instance was spawned from the map.
```c#
virtual bool IsLocalPawn { get; } 
```
Will return true if we're clientside, this entity has an owner and we're
currently treating this owner as the local client. This means the player
could be being spectated.
```c#
virtual bool IsValid { get; } 
```
ImplementsIValid.IsValidReturnstrueif this entity has not been destroyed and it is valid to access its internals
```c#
virtual Vector3 LocalPosition { get; set; } 
```
The entity's position relative to its parent (or the world if no parent)
```c#
virtual Rotation LocalRotation { get; set; } 
```
The entity's local rotation
```c#
virtual float LocalScale { get; set; } 
```
The entity's scale relative to its parent's scale. 1 is normal.
```c#
virtual Vector3 LocalVelocity { get; set; } 
```
Velocity in local coordinates.
```c#
virtual string Name { get; set; } 
```
The entity target name. This is typically used by Entity IO and to generally access specific entities from code.
```c#
virtual Entity Owner { get; set; } 
```
ImplementsIEntity.OwnerThe entity that owns this entity. For example, a pawn's weapon will be owned by its pawn.
```c#
virtual Entity Parent { get; set; } 
```
ImplementsIEntity.ParentWhat this entity is parented to, if anything. Will make this entity move with it's parent, but loses collisions.
```c#
virtual Vector3 Position { get; set; } 
```
ImplementsIEntity.PositionThe entity's world position
```c#
virtual Entity Root { get; } 
```
Gets the top most parent entity. If we don't have a parent, it might be us.
```c#
virtual Rotation Rotation { get; set; } 
```
ImplementsIEntity.RotationThe entity's world rotation
```c#
virtual float Scale { get; set; } 
```
The scale of the entity. 1 is normal.
```c#
virtual Transform Transform { get; set; } 
```
ImplementsIEntity.TransformEntity's transform from world origin.
```c#
virtual Vector3 Velocity { get; set; } 
```
ImplementsIEntity.VelocityThe velocity in world coordinates.
```c#
virtual BBox WorldSpaceBounds { get; } 
```
ImplementsIEntity.WorldSpaceBoundsEntity's axis-aligned bounding box (AABB) in world space.
```c#
Vector3 BaseVelocity { get; set; } 
```
Generally describes the velocity of this object that is caused by its parent moving.
Examples would be conveyor belts and elevators.
```c#
IReadOnlyList<Entity> Children { get; } 
```
All entities that are parented to this entity.
```c#
EntityDebugFlags DebugFlags { get; set; } 
```
Debug flags, to turn on various overlays for entities
```c#
bool EnableDrawing { get; set; } 
```
Turning this off will completely prevent the entity from drawing
```c#
bool EnableHideInFirstPerson { get; set; } 
```
Hide this model when in first person, or our parent is in first person
```c#
bool EnableLagCompensation { get; set; } 
```
Whether or not this entity will be considered for lag compensation. If this is true, the entity's collision bounds
and any hitboxes it has will be rewound to the positions the client saw them in when sending its input command.
```c#
bool EnableShadowCasting { get; set; } 
```
Don't cast no shadow
```c#
bool EnableShadowInFirstPerson { get; set; } 
```
Render Shadows when hidden due to being in first person
```c#
bool EnableShadowOnly { get; set; } 
```
Render only shadows
```c#
bool EnableShadowReceive { get; set; } 
```
Don't receive no shadow [TODO: DOESNT WORK]
```c#
bool EnableViewmodelRendering { get; set; } 
```
Enable Viewmodel Rendering
```c#
Entity GroundEntity { get; set; } 
```
What this entity is "standing" on.
```c#
float Health { get; set; } 
```
Entity's health.
```c#
bool IsPawn { get; } 
```
Returnstrueif this entity has a client and is that client's pawn
```c#
bool IsWorld { get; } 
```
Returnstrueif this entity is the world
```c#
Entity LastAttacker { get; set; } 
```
The entity which attacked this one last. Server only.
```c#
Entity LastAttackerWeapon { get; set; } 
```
The weaponEntity.LastAttackerwas carrying, if any. Server only.
```c#
LifeState LifeState { get; set; } 
```
Entity's life state. Can be used to determine if certain events such asEntity.OnKilledneed firing.
```c#
IReadOnlyDictionary<int, Var> NetworkDictionary { get; } 
```
Here for debug purposes
```c#
PhysicsGroup PhysicsGroup { get; } 
```
If this entity has multiple physics objects, a physics group lets you control them all as one.
```c#
bool Predictable { get; set; } 
```
Defaults totrue, this allows you to turn off prediction for this entity. If you set this
tofalsethen the entity won't be predicted even if it's eligible (has local client owner).
```c#
SceneWorld Scene { get; } 
```
Returns the scene world for the spawn group this entity is in
```c#
TransmitType Transmit { get; set; } 
```
When should this entity and its properties be networked to all clients?
```c#
override int NetworkIdent { get; } 
```
OverridesBaseNetworkable.NetworkIdentShould return an ID of this networkable that is common across the network
## Methods

```c#
static T CreateByName<T,>( string name) 
```
Creates an entity by it's classname
```c#
static Entity CreateByName( string name) 
```
Creates an entity by it's classname
```c#
static IEnumerable<Entity> FindAllByName( string name) 
```
Finds all entities by givenEntity.Name.
```c#
static Entity FindByIndex( int index) 
```
Finds an entity by itsEntity.NetworkIdent.
```c#
static T FindByIndex<T,>( int index) 
```
Finds an entity by itsEntity.NetworkIdent.
```c#
static Entity FindByName( string name, Entity fallback = null) 
```
Finds entities byEntity.Nameand returns the first found result, if one was found. This does not handle cases where there are multiple entities with a given name.
```c#
static IEnumerable<Entity> FindInBox( BBox box) 
```
Find all entities in a box (AABB).
```c#
static IEnumerable<Entity> FindInSphere( Vector3 position, float radius) 
```
Find entities in a sphere.
```c#
static IDisposable LagCompensation( ) 
```
Enable lag compensation. This will rewind all eligible entities to the positions they
were when the client sent the command that is being simulated. When used in ausingblock,
lag compensation will be automatically finished when it is disposed.
```c#
static Entity Read( BinaryReader reader) 
```
Try to read an entity from a binary reader by reading aEntity.NetworkIdentand trying to find an entity with the read id.
```c#
virtual void AddConnection( string outputName, EntityTarget target, string inputName, string overrideParam = "", float delay = 0, int timesToFire = 0) 
```
Adds an Entity IO connection between this entity and target entity.
```c#
virtual void AddOutputEvent( string name, StandardOutputDelegate method, float delay = 0) 
```
Adds a callback to an entity output.
```c#
virtual void BuildInput( ) 
```
Pawns get a chance to mess with the input. This is called on the client.
```c#
virtual void ClientSpawn( ) 
```
Called when the entity spawns on client.
```c#
virtual void Delete( ) 
```
ImplementsIEntity.DeleteDelete this entity. You shouldn't access it anymore.
```c#
virtual void EndTouch( Entity other) 
```
An entity has stopped touching this trigger entity. RequiresEnableTouchenabled on this entity.
```c#
virtual bool FireInput( string input, IEntity activator, object value = null) 
```
Try to fire this Entity IO input
```c#
virtual ValueTask FireOutput( string output, Entity activator, object value = null, float delay = 0) 
```
Try to fire this Entity IO output
```c#
virtual void FrameSimulate( IClient cl) 
```
Called each frame clientside only on Pawn (and anything the pawn decides to call it on).
```c#
virtual void OnActive( ) 
```
Entity is active (clientside). This is called after spawn.
```c#
virtual void OnChildAdded( Entity child) 
```
Called when an entity is parented to this entity.
```c#
virtual void OnChildRemoved( Entity child) 
```
Called when an entity is unparented from this entity.
```c#
virtual void OnClientActive( IClient client) 
```
Called when a player becomes active
```c#
protected virtual void OnComponentAdded( EntityComponent component) 
```
A component has been added to the entity.
```c#
protected virtual void OnComponentRemoved( EntityComponent component) 
```
A component has been removed from the entity.
```c#
protected virtual void OnDestroy( ) 
```
Called when the entity was destroyed. This is not the same as the class destructor.
```c#
virtual void OnKilled( ) 
```
Called (fromEntity.TakeDamageby default unless overridden) when there's no health left.
```c#
virtual void OnNetworkActive( ) 
```
Entity has re-entered the client's visibility and has started receiving network updates again.
```c#
virtual void OnNetworkDormant( ) 
```
The entity has left the client's visibility and has stopped receiving network updates.
When it becomes active again OnNetworkActive will be called.
```c#
protected virtual void OnPhysicsCollision( CollisionEventData eventData) 
```
Called when this entity collides with anything else via Physics.
```c#
protected virtual void OnTagAdded( string tag) 
```
Called when a tag was added to this entity. On the client this will get called
when an entity is created or enters PVS. The passed tag will always be lowercase.
```c#
protected virtual void OnTagRemoved( string tag) 
```
Called when a tag was removed from this entity. The passed tag will always be lowercase.
```c#
virtual Sound PlaySound( string soundName, string attachment) 
```
Play a sound from this entity at given attachment point, updating sounds' position as the entity and its attachments move.
```c#
virtual void SetParent( Entity entity, string attachmentOrBoneName = null, Transform? transform = null) 
```
Become a child of this entity and follow this attachment or bone if provided.
```c#
virtual void SetParent( Entity entity, int bone, Transform? transform = null) 
```
Finds the bone name and calls the other SetParent with it.
```c#
virtual void Simulate( IClient cl) 
```
Called when simulating as part of a player's tick. Like if it's a pawn.
```c#
virtual void Spawn( ) 
```
Called when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
```c#
virtual void StartTouch( Entity other) 
```
An entity has started touching this trigger entity. RequiresEnableTouchenabled on this entity.For solid collisions, seeEntity.OnPhysicsCollision.
```c#
virtual void TakeDamage( DamageInfo info) 
```
Called when the entity receives a damage event. This is where you want to subtract health, etc.
```c#
virtual void Touch( Entity other) 
```
An entity has touched this trigger entity. RequiresEnableTouchenabled on this entity.See alsoModelEntity.EnableTouchPersists.
```c#
void ApplyAbsoluteImpulse( Vector3 impulse) 
```
CallsPhysicsBody.ApplyImpulseon all bodies of this entity with world-space input.
```c#
void ApplyLocalAngularImpulse( Vector3 impulse) 
```
CallsPhysicsBody.ApplyAngularImpulseon all bodies of this entity.
```c#
void ApplyLocalImpulse( Vector3 impulse) 
```
CallsPhysicsBody.ApplyImpulseon all bodies of this entity local-space input. (Relative to the entity)
```c#
protected void CollisionRulesChanged( ) 
```
Internal only: update all of the collision rules, push those rules onto physics shapes.
```c#
Task DeleteAsync( float fTime) 
```
Delete the entity after given delay in seconds.
```c#
Sound PlaySound( string soundName) 
```
Play a sound from this entity, updating sounds' position as the entity moves.
```c#
void RemoveAllDecals( ) 
```
TODO: Implement me.
```c#
void RenderDirty( ) 
```
Mark render dirty
```c#
void ResetInterpolation( ) 
```
Reset the interpolation.
You can use this so if you move an entity it doesn't interpolate to the new position.
```c#
void SetParent( Entity entity, bool boneMerge) 
```
Set the parent to the passed entity
```c#
void Write( BinaryWriter writer) 
```
Write this entity to a binary writer using itsEntity.NetworkIdent, or -1 if the entity is not valid.
```c#
override string ToString( ) 
```
OverridesObject.ToString
## Extensions

```c#
void CopyBonesFrom( Entity ent) 
```
Copy the bones from the target entity, but at the current entity's position and rotation
```c#
void CopyBonesFrom( Entity ent, Vector3 pos, Rotation rot, float scale = 1) 
```
Copy the bones from the target entity, but at this position and rotation instead of the target entity's
```c#
void SetRagdollVelocityFrom( Entity fromEnt, float delta = 0.1, float linearAmount = 1, float angularAmount = 1) 
```
Set the velocity of the ragdoll entity by working out the bone positions of from delta seconds ago
## Nested Types

## Inheriting Types

