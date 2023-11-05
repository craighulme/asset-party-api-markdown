# IComponentSystem

## 
```c#
Is interface
```

## Summary

The amount of components, including disabled
## Properties

```c#
abstract int Count { get; } 
```
The amount of components, including disabled
## Methods

```c#
abstract bool Add( IComponent component) 
```
Add component to this system
```c#
abstract T Create<T,>( bool startEnabled = true) 
```
Create the component
```c#
abstract T Get<T,>( bool includeDisabled = false) 
```
Get a component by type, if it exists
```c#
abstract IEnumerable<T> GetAll<T,>( bool includeDisabled = false) 
```
Get all components by type, if any exist
```c#
abstract T GetOrCreate<T,>( bool startEnabled = true) 
```
Get the component, create if it doesn't exist. Will include disabled components in search.
```c#
abstract bool Remove( IComponent component) 
```
Remove given component from this system
```c#
abstract void RemoveAll( ) 
```
Remove all components to this entity
```c#
abstract bool RemoveAny( Type t) 
```
Remove all components of given type
```c#
abstract bool RemoveAny<T,>( ) 
```
Remove all components of given type
```c#
abstract bool TryGet<T,>( out T component, bool includeDisabled = false) 
```
Returns true if component was found, else false
