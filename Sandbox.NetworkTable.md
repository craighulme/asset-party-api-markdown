# NetworkTable

## 
```c#
Implements IValid
```

## Summary

Each entity has a network table
## Constructors

```c#
NetworkTable( Entity entity) 
```
No Summary
## Properties

```c#
virtual bool IsValid { get; } 
```
ImplementsIValid.IsValidWhether this object is valid or not.
## Methods

```c#
bool CanWrite( bool predicted) 
```
Can write under specific conditions
```c#
void Clear( ) 
```
Erase everything from the network tables
```c#
List<Var> CollectVariables( INetworkTable source, bool deterministic) 
```
No Summary
```c#
void Register<T,>( ref T var, string name, bool predicted, bool local) 
```
No Summary
