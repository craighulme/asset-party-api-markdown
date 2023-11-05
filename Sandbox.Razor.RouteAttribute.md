# RouteAttribute

## 
```c#
Derives from Attribute
```

## Summary

The url split into parts (ie "home" "section" "page" )
## Constructors

```c#
RouteAttribute( string url) 
```
No Summary
## Properties

```c#
string[] Parts { get; } 
```
The url split into parts (ie "home" "section" "page" )
```c#
string Url { get; } 
```
The full url of this route (ie "/home/section/page")
## Methods

```c#
static ValueTuple<TypeDescription, RouteAttribute>? FindValidTarget( string url, string parentUrl) 
```
Given a URL, check out TypeLibrary and find a valid target
```c#
IEnumerable<ValueTuple<string, string>> ExtractProperties( string url) 
```
Given a Url, check for  and convert them to key values
```c#
bool IsUrl( string url) 
```
True if this matches the passed in url.
Queries are trimmed and ignored( ?query=fff )Variables are tested (but not type matched or anything)
