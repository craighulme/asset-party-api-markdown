# AssetTags

## 
```c#
Implements IEnumerable<string>
```

## Summary

Represents a collection of tags for an asset.
This is only necessary so we can save tags as soon as they are added.
## Methods

```c#
virtual IEnumerator<string> GetEnumerator( ) 
```
ImplementsIEnumerable`1.GetEnumerator
```c#
void Add( string tag) 
```
Add a single tag.
```c#
void Add( string[] in_tags) 
```
Add multiple tags at once.
```c#
bool Contains( string tag) 
```
Returns whether this asset has given tag.
```c#
string[] GetAll( ) 
```
Returns all tags of this asset.
```c#
void Remove( string tag) 
```
Remove given tag from the asset.
```c#
void Set( string tag, bool set) 
```
Set or remove the tag based on second argument.
```c#
void Toggle( string tag) 
```
Remove the tag if present, add if not.
## Referencing Members

```c#
AssetTags = Asset.Tags { get; } 
```
