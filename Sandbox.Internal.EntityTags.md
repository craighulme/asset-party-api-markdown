# EntityTags

## Derives from ValueType

## Summary

Entity Tags are strings you can set and check for on any entity. Internally
these strings are tokenized and networked so they're also available clientside.
## Properties

```c#
IReadOnlyCollection<string> List { get; } 
```
Returns all the tags this entity has. We can't let you modify the HashSet directly
because we need to keep in sync with an engine version.
## Methods

```c#
void Add( string tag) 
```
Try to add the tag to this entity.
```c#
void Add( string[] tags) 
```
Adds multiple tags. CallsEntityTags.Addfor each tag.
```c#
void Clear( ) 
```
Remove all tags
```c#
bool Has( string tag) 
```
Returns true if this entity has given tag.
```c#
bool HasAny( HashSet<string> tagList) 
```
Returns true if this entity has one or more tags from given tag list.
```c#
void Remove( string tag) 
```
Try to remove the tag from this entity.
```c#
void Set( string tag, bool on) 
```
Removes or adds a tag based on the second argument.
```c#
void Toggle( string tag) 
```
Removes a tag if it exists, adds it otherwise.
## Referencing Members

```c#
readonly EntityTags = Entity.Tags
```
