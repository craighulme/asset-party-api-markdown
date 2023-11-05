# SandboxBaseExtensions

## 
```c#
Derives from object
```

## Summary

Extensions for Model
## Methods

```c#
static void Add( VertexBuffer self, Vector3 pos) 
```
Add a vertex using this position and everything else from Default
```c#
static void Add( VertexBuffer self, Vector3 pos, Vector2 uv) 
```
Add a vertex using this position and UV, and everything else from Default
```c#
static void AddCube( VertexBuffer self, Vector3 center, Vector3 size, Rotation rot, Color32 color = null) 
```
Add a cube to the vertex buffer. Will include indices if they're enabled.
```c#
static void AddQuad( VertexBuffer self, Rect rect) 
```
Add a quad to the vertex buffer. Will include indices if they're enabled.
```c#
static void AddQuad( VertexBuffer self, Vertex a, Vertex b, Vertex c, Vertex d) 
```
Add a quad to the vertex buffer. Will include indices if they're enabled.
```c#
static void AddQuad( VertexBuffer self, Vector3 a, Vector3 b, Vector3 c, Vector3 d) 
```
Add a quad to the vertex buffer. Will include indices if they're enabled.
```c#
static void AddQuad( VertexBuffer self, Ray origin, Vector3 width, Vector3 height) 
```
Add a quad to the vertex buffer. Will include indices if they're enabled.
```c#
static void AddTriangle( VertexBuffer self, Vertex a, Vertex b, Vertex c) 
```
Add a triangle to the vertex buffer. Will include indices if they're enabled.
```c#
static void CopyBonesFrom( Entity self, Entity ent) 
```
Copy the bones from the target entity, but at the current entity's position and rotation
```c#
static void CopyBonesFrom( Entity self, Entity ent, Vector3 pos, Rotation rot, float scale = 1) 
```
Copy the bones from the target entity, but at this position and rotation instead of the target entity's
```c#
static Particles DoBulletImpact( Surface self, TraceResult tr) 
```
Create a particle effect and play an impact sound for this surface being hit by a bullet
```c#
static void DoFootstep( Surface self, Entity ent, TraceResult tr, int foot, float volume) 
```
Create a footstep effect
```c#
static List<T> GetAllData<T,>( Model self) 
```
Returns all game data nodes that derive from given class/interface, and are present on the model. Does NOT support data nodes that allow multiple entries.
```c#
static void ProceduralHitReaction( AnimatedEntity self, DamageInfo info, float damageScale = 1) 
```
Sets the procedural hit creation parameters for the animgraph node, which makes the
model twitch according to where it got hit.The parameters set arebool hit
int hit_bone
vector hit_offset
vector hit_direction
vector hit_strength
```c#
static void SetRagdollVelocityFrom( Entity self, Entity fromEnt, float delta = 0.1, float linearAmount = 1, float angularAmount = 1) 
```
Set the velocity of the ragdoll entity by working out the bone positions of from delta seconds ago
