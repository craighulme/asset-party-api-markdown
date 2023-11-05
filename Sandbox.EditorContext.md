# EditorContext

## 
```c#
Derives from object
```

## Summary

If the current entity we're drawing selected
## Constructors

```c#
protected EditorContext( ) 
```
No Summary
## Properties

```c#
virtual bool IsSelected { get; } 
```
If the current entity we're drawing selected
```c#
virtual EntityObject Target { get; } 
```
The current entity we're rendering gizmos for
```c#
HashSet<EntityObject> Selection { get; } 
```
All selected entities
## Methods

```c#
virtual EntityObject FindTarget( string name) 
```
Given a string name return the first found target
```c#
virtual EntityObject[] FindTargets( string name) 
```
Given a string name return all found targets
## Nested Types

