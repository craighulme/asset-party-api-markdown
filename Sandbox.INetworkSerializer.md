# INetworkSerializer

## 
```c#
Is interface
```

## Summary

Manually network a class or a struct via theReadandWritemethods.The class/struct would still need to be used on a property with[Net]attribute.
## Methods

```c#
abstract void Read( ref NetRead read) 
```
Read an instance of this class from aSandbox.NetReader.
```c#
abstract void Write( NetWrite write) 
```
Write an instance of this class to aSandbox.NetWriter.
