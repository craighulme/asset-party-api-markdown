# Http

## 
```c#
Implements IDisposable
```

## Summary

ImplementsIDisposable.Dispose
## Constructors

```c#
Http( Uri uri) 
```
No Summary
## Fields

```c#
static string Origin = https://sbox.facepunch.com/
```
No Summary
```c#
static string UserAgent = facepunch-s&box
```
No Summary
## Properties

```c#
Uri Uri { get; } 
```
No Summary
## Methods

```c#
static bool AreHeadersAllowed( Dictionary<string, string> headers) 
```
No Summary
```c#
static bool IsAllowed( Uri uri) 
```
No Summary
```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.Dispose
```c#
void AddHeader( string key, string value) 
```
No Summary
```c#
Task<byte[]> GetBytesAsync( ) 
```
No Summary
```c#
Task<Stream> GetStreamAsync( ) 
```
No Summary
```c#
Task<string> GetStringAsync( ) 
```
No Summary
