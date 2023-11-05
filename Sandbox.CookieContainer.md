# CookieContainer

## 
```c#
Derives from object
```

## Summary

Load JSON encodable data from cookies
## Methods

```c#
T Get<T,>( string key, T fallback) 
```
Load JSON encodable data from cookies
```c#
string GetString( string key, string fallback = "") 
```
Get a stored session cookie.
```c#
void Set<T,>( string key, T value) 
```
Set JSON encodable object to data
```c#
void SetString( string key, string value) 
```
Set a cookie to be stored between sessions. The cookie will expire one month
from when it was set.
```c#
bool TryGetString( string key, out string val) 
```
Get a stored session cookie.
