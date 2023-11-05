# Pair

## ```c#
Derives from ValueType
```

## Summary

Describes target collisionPair.Resultbetween two objects with given tags.
## Constructors

```c#
Pair( string l, string r, Result x) 
```
No Summary
## Properties

```c#
string Left { get; set; } 
```
A tag representing one of the objects in a collision pair.
```c#
Result Result { get; set; } 
```
Target collision result when two objects collide, each with tags set inPair.LeftandPair.Right.
```c#
string Right { get; set; } 
```
A tag representing the other object in a collision pair.
## Methods

```c#
bool Any( string left) 
```
Return true if either match
```c#
bool Is( string left, string right) 
```
Return true if these match in either order
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
## Referencing Members

```c#
HashSet<Pair> = CollisionRules.Pairs { get; set; } 
```
