# IHotloadManaged

## ```c#
Is interface
```

## Summary

During hotloads, instances of types implementing this interface will be notified when
they get replaced.
## Methods

```c#
virtual void Created( IReadOnlyDictionary<string, object> state) 
```
Called when this instance has been created during a hotload, replacing an
instance from an older version of the containing assembly. Thestateparameter will contain any values populated whenIHotloadManaged.Destroyedwas called
on the old instance that was replaced.
```c#
virtual void Destroyed( Dictionary<string, object> state) 
```
Called when this instance is about to be replaced during a hotload.
The implementor may optionally write to thestatedictionary, which gets passed to the new replacing instance whenIHotloadManaged.Createdis called on it.
```c#
virtual void Failed( ) 
```
Called when this instance could not be upgraded during a hotload, and any references
to it have been replaced with null. This is a good time to clean up any unmanaged resources
related to this instance.
