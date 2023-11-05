# LineAttribute

## 
```c#
Derives from MetaDataAttribute
```

## Summary

Draws a line in Hammer. You can have multiple of this attribute.
## Constructors

```c#
LineAttribute( string startKey, string startKeyValue, bool onlySelected = false) 
```
Draws lines between this entity and all entities which have a key named 'startKey' and its value matches
the value of our 'startKeyValue'.
```c#
LineAttribute( string startKey, string startKeyValue, string endKey, string endKeyValue, bool onlySelected = false) 
```
Draws lines between all entities, starting from each entity that has a key named 'startKey' and its value matches
the value of our 'startKeyValue' and going to each entity that has a key namedendKeywith a value of 'endKeyValue's value.
## Methods

```c#
override void AddHelpers( List<Tuple<string, string[]>> helpers) 
```
OverridesMetaDataAttribute.AddHelpers
