# Entry

## ```c#
Derives from object
```

## Summary

No Summary
## Constructors

```c#
Entry( ) 
```
No Summary
## Properties

```c#
string Class { get; set; } 
```
No Summary
```c#
List<Entry> Components { get; set; } 
```
No Summary
```c#
List<Entry> Entities { get; set; } 
```
No Summary
```c#
string Guid { get; set; } 
```
No Summary
```c#
CaseInsensitiveDictionary<Key> Keys { get; set; } 
```
No Summary
## Methods

```c#
T GetValue<T,>( string name, T defaultValue = null) 
```
No Summary
```c#
void SetValue<T,>( string name, T value) 
```
No Summary
```c#
bool TryGetValue<T,>( string name, out T outValue) 
```
No Summary
