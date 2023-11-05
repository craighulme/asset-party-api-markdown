# ITagSet

## Is interface

## Summary

Add a tag to the set.
## Methods

```c#
abstract void Add( string tag) 
```
Add a tag to the set.
```c#
abstract bool Has( string tag) 
```
Does this set have the specified tag?
```c#
abstract void Remove( string tag) 
```
Remove a tag from the set.
```c#
abstract void RemoveAll( ) 
```
Remove all tags from the set.
```c#
virtual void Set( string tag, bool state) 
```
Add or remove this tag, based on state
```c#
virtual void SetFrom( ITagSet set) 
```
Set the tags to match this other tag set
```c#
virtual void Toggle( string tag) 
```
If this tag is already here, remove it, else add it.
```c#
abstract IEnumerable<string> TryGetAll( ) 
```
Try to get all tags in the set.
