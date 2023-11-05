# IModelBreakCommand

## ```c#
Is interface
```

## Summary

A model break command, applied in ModelDoc and ran after spawning model gibs. The inheriting class must have a LibraryAttribute.
## Methods

```c#
abstract void OnBreak( Result result) 
```
This will be called after an entity with this model breaks viaBreakablesclass.
