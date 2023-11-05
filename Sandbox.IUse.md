# IUse

## Is interface

## Summary

If an entity implements this it'll be interactable, typically by looking at it and pressing the USE button,
but the implementation will depend on the currently active game.
## Methods

```c#
abstract bool IsUsable( Entity user) 
```
Dictates whether this entity is usable by given user.
```c#
abstract bool OnUse( Entity user) 
```
Called when the (probably) player has used this entity.
