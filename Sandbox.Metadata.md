# Metadata

## 
```c#
Derives from object
```

## Summary

A simple class for storing and retrieving metadata values.
## Constructors

```c#
Metadata( ) 
```
No Summary
## Methods

```c#
T GetValueOrDefault<T,>( string key, T defaultValue = null) 
```
Get the a value. If it's missing or the wrong type then use the default value.
```c#
void SetValue( string key, object value) 
```
Set a value with the specified key.
```c#
bool TryGetValue<T,>( string key, out T outValue) 
```
Try to get a value of the specified type.
