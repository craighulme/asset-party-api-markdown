# PlayerStat

## 
```c#
Derives from ValueType
```

## Summary

The description of this stat, as defined on the backend
## Properties

```c#
string Description { get; init; } 
```
The description of this stat, as defined on the backend
```c#
string Name { get; init; } 
```
The programatic name for this stat. This should probably be called Ident
```c#
string Title { get; init; } 
```
The title of this stat, as defined on the backend
```c#
string Unit { get; init; } 
```
The unit of this stat as defined on the backend
```c#
double Value { get; init; } 
```
The current stat value
```c#
string ValueString { get; init; } 
```
The current value formatted using Unit
## Referencing Members

```c#
PlayerStat = PlayerStats.Get( string ) 
```
```c#
virtual IEnumerator<PlayerStat> = PlayerStats.GetEnumerator( ) 
```
```c#
PlayerStat = PlayerStats.Item[ string propertyName, ] { get; } 
```
