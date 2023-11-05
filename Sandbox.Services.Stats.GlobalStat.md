# GlobalStat

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
long Players { get; init; } 
```
The amount of players that have this stat
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
```c#
double Velocity { get; init; } 
```
The change in this stat in units per hour
## Referencing Members

```c#
GlobalStat = GlobalStats.Get( string ) 
```
```c#
virtual IEnumerator<GlobalStat> = GlobalStats.GetEnumerator( ) 
```
```c#
GlobalStat = GlobalStats.Item[ string propertyName, ] { get; } 
```
