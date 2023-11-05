# RenderEntity

## 
```c#
Derives from Entity
```

## Summary

Render bounds of this entity. It will not render unless this AABB is on the screen.
## Constructors

```c#
RenderEntity( ) 
```
No Summary
## Fields

```c#
BBox RenderBounds
```
Render bounds of this entity. It will not render unless this AABB is on the screen.
## Methods

```c#
virtual void DoRender( SceneObject obj) 
```
Render this entity. Here's some warnings:This is called in a thread. Don't create/delete/move entities in this loopThis can be called multiple times per frame for different scene layers. For example, once to
draw the shadow caster, once to draw the opaque object, once to draw the transparent object.
Obviously which of these get called depends on your object setup. Check Render.Layer to
determine which layer is being rendered.
```c#
protected virtual void Think( ) 
```
CallsRenderEntity.UpdateSceneObjectevery frame. You probably want to override that.
```c#
virtual void UpdateSceneObject( SceneObject obj) 
```
Keep the scene object updated. By default this moves the transform to match this entity's transform
and updates the bounds to the new position.
```c#
override void OnActive( ) 
```
OverridesEntity.OnActiveEntity is active (clientside). This is called after spawn.
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
