# ModelArchetype

## Derives from Enum

## Summary

Default model archetypes.
These types are defined in "tools/model_archetypes.txt".
## Fields

```c#
static ModelArchetype animated_model = 2
```
Animated model. Typically no physics.
```c#
static ModelArchetype breakable_prop_model = 16
```
A physics model that can be broken into other physics models.
```c#
static ModelArchetype generic_actor_model = 32
```
A generic actor/NPC model.
```c#
static ModelArchetype jointed_physics_model = 8
```
A ragdoll type model.
```c#
static ModelArchetype physics_prop_model = 4
```
A generic physics enabled model.
```c#
static ModelArchetype static_prop_model = 1
```
A static model. It can still have collisions, but they do not have physics.
## Referencing Members

```c#
ModelArchetype = ModelAttribute.Archetypes { get; set; } 
```
