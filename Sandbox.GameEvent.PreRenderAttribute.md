# PreRenderAttribute

## ```c#
Derives from EventAttribute
```

## Summary

Called right before rendering. All entities are in the position they're going to be rendered in. Moving entities
here will have no effect until the next frame. Moving SceneObjects is possible here and they will be rendered in their
new positions.
## Constructors

```c#
PreRenderAttribute( ) 
```
No Summary
