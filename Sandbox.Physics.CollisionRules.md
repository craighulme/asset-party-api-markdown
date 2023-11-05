# CollisionRules

## 
```c#
Derives from object
```

## Summary

This is a JSON serializable description of the physics's collision rules. This allows us to send it
to the engine - and store it in a string table (which is networked to the client). You shouldn't really
ever have to mess with this, it's just used internally.
## Constructors

```c#
CollisionRules( ) 
```
No Summary
## Properties

```c#
Dictionary<string, Result> Defaults { get; set; } 
```
If no pair matching is found, this is what we'll use
```c#
HashSet<Pair> Pairs { get; set; } 
```
What happens when a pair collides
## Methods

```c#
void Clean( ) 
```
Remove duplicates etc
## Nested Types

