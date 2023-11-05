# BaseNetworkable

## ```c#
Implements INetworkTable
```

## Summary

A network capable object.Properties marked with[Net]attribute will be automagically networked to clients when possible.
## Constructors

```c#
BaseNetworkable( ) 
```
No Summary
## Properties

```c#
virtual int NetworkIdent { get; } 
```
Should return an ID of this networkable that is common across the network
```c#
string ClassName { get; protected set; } 
```
The "class name" used internally for identifying networkables.
## Methods

```c#
virtual void BuildNetworkTable( NetworkTable table) 
```
ImplementsINetworkTable.BuildNetworkTableThis method is overridden by codegen to make certain network features like[Net]functional. It is not meant to be used directly unless you know what you are doing.
```c#
void WriteNetworkData( ) 
```
Serialize this class to the network. You shouldn't need to call this manually unless you're
implementing INetworkSerializer and want to force a write. In other situations we can detect
when things change and update them manually.
## Inheriting Types

