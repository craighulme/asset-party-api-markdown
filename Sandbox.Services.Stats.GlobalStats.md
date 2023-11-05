# GlobalStats

## Derives from object
Implements IEnumerable< GlobalStat>

## Summary

True if we're currently fetching new stats
## Properties

```c#
bool IsRefreshing { get; } 
```
True if we're currently fetching new stats
```c#
DateTime LastRefresh { get; } 
```
The UTC datetime when we last fetched new stats
## Methods

```c#
virtual IEnumerator<GlobalStat> GetEnumerator( ) 
```
ImplementsIEnumerable`1.GetEnumerator
```c#
GlobalStats Copy( ) 
```
Make a copy of this class. Allows you to store the stats from a point in time.
```c#
GlobalStat Get( string name) 
```
Get a stat by name. Will return an empty stat if not found
```c#
Task Refresh( ) 
```
Refresh these global stats - grab the latest values
```c#
bool TryGet( string name, out GlobalStat stat) 
```
Get a stat by name, returns true if found
## Operators

```c#
GlobalStat this[ string propertyName, ] 
```
No Summary
