# ParticleAttachment

## 
```c#
Derives from Enum
```

## Summary

Create on attachment point, but don't follow
## Fields

```c#
static ParticleAttachment Attachment = 4
```
Create on attachment point, but don't follow
```c#
static ParticleAttachment AttachmentFollow = 5
```
Create on attachment point, and update to follow the attachment point
```c#
static ParticleAttachment Bone = 14
```
Create on bone, but don't follow
```c#
static ParticleAttachment BoneFollow = 15
```
Create on bone, and update to follow the bone.
```c#
static ParticleAttachment CenterFollow = 13
```
Create at center of entity's bounds (Entity.WorldSpaceBounds), and update to follow the entity
```c#
static ParticleAttachment CustomOrigin = 2
```
Create at a custom origin, but don't follow
```c#
static ParticleAttachment CustomOriginFollow = 3
```
Create at a custom origin, follow relative position to specified entity
```c#
static ParticleAttachment EyesFollow = 6
```
Create on eyes of the attached entity, and update to follow the entity
```c#
static ParticleAttachment Invalid = -1
```
Invalid particle attachment type.
```c#
static ParticleAttachment Origin = 0
```
Create at entity's origin, but don't follow
```c#
static ParticleAttachment OriginFollow = 1
```
Create at entity's origin, and update to follow the entity
```c#
static ParticleAttachment OverheadFollow = 7
```
Create at the top of the entity's model bounds. (Model.Bounds)
```c#
static ParticleAttachment RenderOriginFollow = 10
```
Create at the renderorigin of the entity, and update to follow
```c#
static ParticleAttachment RootBoneFollow = 9
```
Create at the root bone of the entity, and update to follow.
```c#
static ParticleAttachment WorldOrigin = 8
```
Used for control points that don't attach to an entity.
## Referencing Members

```c#
ParticleAttachment = ModelParticle.AttachmentType { get; set; } 
```
```c#
void Particles.SetEntityAttachment( int, Entity, string, Vector3, ParticleAttachment ) 
```
